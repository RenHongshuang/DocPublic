# Hash

## 1.引入

如果让你在100万个身份证号中找出两个一样的你怎么做？

可能会想到暴力?

```
1.恐怖的暴力2层循环 
long long int data[SIZE];
for(int i =0;i<SIZE;i++){
	for(int j =i+1;j<SIZE;i++){
		if(data[i]==data[j]){
		rerturn 1;	
		}
	}
}
return0;
```

还可能会想到频率统计？

```
2. 频率统计
// 取值范围时0~10
// SIZE 10;
for(int i =0;i<SIZE;i++){
	cin >>tmp;
	data[tmp]++;
}
但是这道题的问题用这种方法是开不出10的18次方的数组，不信你试试?
```

正确的解法是用hash table

思路：建立一个数组+链表的hash表，拿到数据先在hash table里查询是否存在一样的
如果没有就插入到表中，如果有就返回结果 ，下面是hash相关的一些套路

```
#define SIZE 1000000

typedef struct Node{
	int value;
	struct Node *next;
}Node;

//hash表

Node HashTable[SIZE +10];

Node HashPool[SIZE + 10];
int HashIndex;

Node * getNewNode(){
	return &HashPool[HashIndex++];
}

void insertNode(int key,Node * newNode){
	newNode->next = HashTable[key].next;
	HashTable[key].next = newNode;
}

int getKey(int val){
	return val % (SIZE +3);
}
```

## 2.例题

 http://poj.org/problem?id=3349

 题目大意：
有0-100000(10万)个雪花，每个雪花有6个花瓣，每个花瓣的取值范围是 0~10000000(0~1千万)
求是否有两个雪花相同(比如两个雪花的花瓣只是顺序不一样，花瓣的数值一样 算一个花瓣)

```
#include <iostream>
using namespace std;

#define SIZE 1000000

typedef struct Node{
	int value[6];
	struct Node *next;
}Node;

//hash表

Node HashTable[SIZE +10];

Node HashPool[SIZE + 10];
int HashIndex;

Node * getNewNode(){
	return &HashPool[HashIndex++];
}

void insertNode(int key,Node * newNode){
	newNode->next = HashTable[key].next;
	HashTable[key].next = newNode;
}

void selectSort(int data[6]){
	int minVal = 0x7FFFFFFF;
	int pos =0;
	for (int i =0;i<6;i++){
		minVal = 0x7FFFFFFF;
		pos =0;
		for (int j =i;j<6;j++){
			if(minVal > data[j]){
				minVal = data[j];
				pos =j;
			}
		}
		int tmp = data[i];
		data[i] = data[pos];
		data[pos]= tmp;
	}
}

int isSame(Node * snow1, Node * snow2){
	for(int i=0;i<6;i++){
		if(snow1->value[i] != snow2->value[i]){
			return 0;		
		}
	}
	return 1;
}

int foundTwins(int key,Node * targetNode){
	selectSort(targetNode->value);
	Node * curNode = HashTable[key].next;
	while(curNode){
		selectSort(curNode->value);
		if(isSame(curNode,targetNode)){
			return 1;
		}
		curNode = curNode ->next;
	}
	return 0;
}


int main(){
	/*
	freopen("input.txt","w",stdout);
	cout <<100000 <<endl;
	for(int i=0;i < 100000 ;i++){
		for(int j=0;j<6;j++){
			cout << (rand()* rand())%10000000<<" ";
		}
		cout<<endl;
	}
	*/

	//freopen("input.text","r",stdin);
	
	
	int SnowNum =0;
	scanf("%d",&SnowNum);

	Node * curNode;
	int key =0;
	int hasTwins =0;
	for(int i=0;i<SnowNum;i++){
		curNode = getNewNode();
		key =0;
		for(int j=0;j<6;j++){
			scanf("%d",&curNode->value[j]);
			key = (key + curNode->value[j]) % (SIZE +3);
		}

		if(foundTwins(key,curNode)){
			hasTwins =1;
			break;
		}else {
			insertNode(key,curNode);
		}

	}
	if(hasTwins){
		cout<<"Twin snowflakes found."<<endl;
	}else {
		cout<<"No two snowflakes are alike."<<endl;	
	}

	return 0;
}
```

