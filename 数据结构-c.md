数据结构（C语言）
===
<!--GFM-TOC -->
## 目录
* [头文件+预定义](#头文件预定义)
* [线性表](#线性表)
    * [顺序表](#顺序表)
        * [1.顺序表存储结构](#1顺序表存储结构)
        * [2.顺序表的初始化](#2顺序表的初始化)
        * [3.顺序表的建立](#3顺序表的建立)
        * [4.顺序表按照位序查找元素的值](#4顺序表按照位序查找元素的值)
        * [5.顺序表中按照结点的值查找结点的位序](#5顺序表中按照结点的值查找结点的位序)
        * [6.顺序表数据元素的插入](#6顺序表数据元素的插入)
        * [7.顺序表数据元素的删除](#7顺序表数据元素的删除)
        * [8.顺序表数据元素的遍历输出](#8顺序表数据元素的遍历输出)
        * [9.顺序表的销毁](#9顺序表的销毁)
    * [单链表](#单链表)
        * [1.单链表存储结构](#1单链表存储结构)
        * [2.单链表的初始化](#2单链表的初始化)
        * [3.单链表的建立（头插法）](#3单链表的建立头插法)
        * [4.单链表的建立（尾插法）](#4单链表的建立尾插法)
        * [5.单链表的遍历输出](#5单链表的遍历输出)
        * [6.单链表结点的插入](#6单链表结点的插入)
        * [7.单链表结点的删除](#7单链表结点的删除)
        * [8.单链表中按照结点的值查找结点的位序](#8单链表中按照结点的值查找结点的位序)
        * [9.单链表中按照结点的位序返回结点的值](#9单链表中按照结点的位序返回结点的值)
        * [10.单链表的销毁](#10单链表的销毁)
        * [11.求单链表的长度](#11求单链表的长度)
        * [12.两个单链表的归并](#12两个单链表的归并)
        * [13.递归实现链表的遍历输出（正序）](#13递归实现链表的遍历输出正序)
        * [14.递归实现链表的遍历输出（逆序）](#14递归实现链表的遍历输出逆序)
        * [15.递归实现链表的逆序](#15递归实现链表的逆序)
        * [16.递归求链表的长度](#16递归求链表的长度)
* [顺序栈](#顺序栈)
    * [1.顺序栈存储结构](#1顺序栈存储结构)
    * [2.顺序栈的初始化](#2顺序栈的初始化)
    * [3.顺序栈的建立](#3顺序栈的建立)
    * [4.判断栈是否为空](#4判断栈是否为空)
    * [5.取栈顶元素](#5取栈顶元素)
    * [6.元素进栈](#6元素进栈)
    * [7.元素出栈](#7元素出栈)
    * [8.计算栈中数据元素的个数](#8计算栈中数据元素的个数)
    * [9.遍历顺序栈](#9遍历顺序栈)
* [循环队列](#循环队列)
    * [1.循环队列存储结构](#1循环队列存储结构)
    * [2.循环队列的初始化](#2循环队列的初始化)
    * [3.循环队列的建立](#3循环队列的建立)
    * [4.判断队列是否为空](#4判断队列是否为空)
    * [5.取队首元素](#5取队首元素)
    * [6.元素入队](#6元素入队)
    * [7.元素出队](#7元素出队)
    * [8.计算队列中数据元素的个数](#8计算队列中数据元素的个数)
    * [9.遍历循环队列](#9遍历循环队列)
* [二叉树](#二叉树)
    * [1.二叉树存储结构](#1二叉树存储结构)
    * [2.二叉树的创建](#2二叉树的创建)
    * [3.二叉树的遍历（前序）](#3二叉树的遍历前序)
    * [4.二叉树的遍历（中序）](#4二叉树的遍历中序)
    * [5.二叉树的遍历（后序）](#5二叉树的遍历后序)
    * [6.二叉树的遍历（层次）](#6二叉树的遍历层次)
    * [7.求二叉树高度](#7求二叉树高度)
    * [8.交换二叉树的左右子树](#8交换二叉树的左右子树)
    * [9.求二叉树的结点个数](#9求二叉树的结点个数)
    * [10.求二叉树的叶子数](#10求二叉树的叶子数)
    * [11.按照目录形式输出二叉树](#11按照目录形式输出二叉树)
    * [12.二叉树的销毁](#12二叉树的销毁)
* [树](#树)
    * [1.树的存储结构](#1树的存储结构)
    * [2.求树的深度](#2求树的深度)
    * [3.树的后根遍历](#3树的后根遍历)
* [查找表](#查找表)
    * [顺序表](#顺序表)
        * [1.查找表的存储结构](#1查找表的存储结构)
        * [2.顺序查找法](#2顺序查找法)
        * [3.折半查找法](#3折半查找法)
    * 二叉查找树
    * 二叉平衡树
    * 哈希表
* [排序表](#排序表)
    * [排序表的存储结构](#排序表的存储结构)
    * [插入排序](#插入排序)
        * [1.直接插入排序](#1直接插入排序)
        * [2.折半排序](#2折半排序)
        * [3.希尔排序](#3希尔排序)
    * [交换排序](#交换排序)
        * [1.起泡排序](#1起泡排序)
        * [2.快速排序](#2快速排序)
    * [选择排序](#选择排序)
        * [1.简单选择排序](#1简单选择排序)
        * [2.堆排序](#2堆排序)
    * 归并排序
    * 基数排序
* [图](#图)
    * [存储结构](#存储结构)
        * [1.邻接矩阵](#1邻接矩阵)
        * [2.邻接表](#2邻接表)
        * 3.有向图十字链表
        * 4.无向图的邻接多重表
    * [深度优先遍历(DFS)](#深度优先遍历dfs)
        * [1.邻接矩阵](#1邻接矩阵)
        * [2.邻接表](#2邻接表)
    * 广度优先遍历(BFS)
    * [构造最小生成树](#构造最小生成树)
        * [1.Prim算法](#1prim算法)
        * [2.Kruskal算法](#2kruskal算法)
    * [有向无环图](#有向无环图)
        * [1.拓扑排序](#1拓扑排序)
        * [2.关键路径](#2关键路径)
    * [最短路径](#最短路径)
        * [1.Dijkstra算法](#1dijkstra算法)
        * [2.Floyd算法](#2floyd算法)
<!--GFM-TOC-->
## 头文件+预定义
```c
#include<stdio.h>
#include<stdlib.h>
#define TRUE 1
#define FALSE 0
#define OK 1
#define ERROR 0
#define OVERFLOW -2
typedef int status;
```

## 线性表

### 顺序表

#### 1.顺序表存储结构
```c
#define LIST_INIT_SIZE 100
#define LISTINCREMENT 10
typedef int Elemtype;
typedef struct
{
    Elemtype *elem;
    int length;
    int listsize;
}SqList;
```

#### 2.顺序表的初始化
```c
Status InitSqList(SqList &L)
{
    L.elem=(ElemType *)malloc(sizeof(ElemType )*LIST_INIT_SIZE);
    if(!L.elem)
        exit(OVERFLOW);
    L.length=0;
    L.listsize=LIST_INIT_SIZE;
    return OK;
}
```

#### 3.顺序表的建立
```c
Status InitSqList(SqList &L,int n)
{
    int i;
    L.elem=(ElemType *)malloc(sizeof(ElemType)*n);
    if(!L.elem)
        exit(OVERFLOW);
    L.length=L.listsize=n;    
    for(i=0;i<n;i++)
        scanf("%d",&L.elem[i]);
    return OK;
}
```

#### 4.顺序表按照位序查找元素的值
```c
Status GetSqList(SqList L,int n,ElemType &e)
{
    if(n>L.length||n<1)  
        return ERROR;
    e=L.elem[n-1];
    return  OK;
}
```

#### 5.顺序表中按照结点的值查找结点的位序
```c
int SearchSqList(SqList L,int x)
{
    int i=1;
    while (i<=L.length&&L.elem[i-1]!=x)
        i++;
    if (i<=L.length)
        return i;
    else
        return 0;
}
```

#### 6.顺序表数据元素的插入
```c
Status InsertSqList(SqList &L,int n, ElemType e) 
{
    int i;
    if(n<1||n>L.length+1)   
        return ERROR;
  
    if(L.length>=L.listsize) 
    {
        ElemType *newbase ;
        newbase=(ElemType*)realloc(L.elem,
                                  (L.listsize+LISTINCREMENT)*sizeof(ElemType));
  
        if(!newbase)
            exit(OVERFLOW);
        L.elem=newbase;
        L.listsize+=LISTINCREMENT;
  
    }
    for(i=L.length;i>n;i--)
        L.elem[i]=L.elem[i-1];
    L.elem[n-1]=e;
    L.length++;
    return OK;
}
```

#### 7.顺序表数据元素的删除
```c
Status DeleteSqList(SqList &L,int n, ElemType &e) 
{
    int i;
    if(n<1||n>L.length)   
        return ERROR;
    e=L.elem[n-1];
    for(i=n-1;i<L.length-1;i++)
        L.elem[i]=L.elem[i+1];
    L.length--;
    return OK;
}
```

#### 8.顺序表数据元素的遍历输出
```c
Status VisitSqList(SqList L)
{
   int i;
   for(i=0;i<L.length;i++) 
       printf("%d ",L.elem[i]);
    printf("\n");
    return OK;
}
```

#### 9.顺序表的销毁
```c
Status DestroySqList(SqList &L)
{
   if (!L.elem)
       return ERROR;
   free(L.elem);
   L.elem=NULL;
   L.length=L.listsize=0;
   return OK;
}
```

### 单链表

#### 1.单链表存储结构
```c
typedef int ElemType;
typedef struct LNode
{
    ElemType data;
    struct LNode *next;
}LNode,*LinkList;
```

#### 2.单链表的初始化
```c
Status InitList(LinkList &L)                 
{
    L=(LNode *)malloc(sizeof(LNode));
    L->next=NULL;
    return OK;
}
```

#### 3.单链表的建立（头插法）
```c
void CreateList(LinkList &L,int n)
{
   int i;
   LinkList p;
   L=(LNode *) malloc(sizeof(LNode));
   L->next=NULL;
   for(i=0;i<n;i++)
   {
        p=(LNode *)malloc(sizeof(LNode));
        scanf("%d",&p->data);
        p->next=L->next;
        L->next=p;
   }
}
```

#### 4.单链表的建立（尾插法）
```c
void CreateList(LinkList &L,int n)
{
   int i;
   LinkList p,q=L;
   L=(LNode *)malloc(sizeof(LNode));
   L->next=NULL;
   for(i=0;i<n;i++)
   {
        p=(LNode *)malloc(sizeof(LNode));
        scanf("%d",&p->data);
        p->next=NULL;
        q->next=p;
        q=p;
   }
}
```

#### 5.单链表的遍历输出
```c
void VisitList(LinkList L)
{
    LinkList p=L->next;
    while(p)
    {
        printf("%d ",p->data);                    
        p=p->next;                                
    }
    printf("\n");
}
```

#### 6.单链表结点的插入
```c
Status InsertList(LinkList&L,int i,ElemType e)
{
    LinkList p=L;
    int j=0;
    while(p&&j<i-1) 
    {
        p=p->next;
        j++;
    }
    if(!p||j>i-1)
        return ERROR;
    LinkList q=(LNode *)malloc(sizeof(LNode));
    q->data=e;
    q->next=p->next;
    p->next=q;
    return OK;
}
```

#### 7.单链表结点的删除
```c
Status DeleteList(LinkList&L,int i,ElemType &e)
{
    LinkList p=L; 
    LinkList q;
    int j=0;
    while(p->next&&j<i-1) 
    {
       p=p->next;
       j++;
    }
    if(!(p->next)||j>i-1)
        return ERROR;
    q=p->next;
    p->next=q->next;
    e=q->data;
    free(q);
    return OK;
  }
 ```

#### 8.单链表中按照结点的值查找结点的位序
```c
Status LocateList(LinkList L,ElemType e)
{
    LinkList p=L->next;
    int i=1;
    while(p&&p->data!=e)
    {
        p=p->next;
        i++;
    }
    if(!p)
        return ERROR;
    else 
        return i;
}
```

#### 9.单链表中按照结点的位序返回结点的值
```c
Status GetList(LinkList L,int i,ElemType &e)
{
    LinkList p=L->next;
    int j=1;
    while(p&&j<i)
    {
        p=p->next;
        j++;
    }
    if(!p||j>i)
        return ERROR;
    e=p->data;
    return OK;
}
```

#### 10.单链表的销毁
```c
Status DestroyList(LinkList &L)
{
   LinkList p,q;
   p=L;
   while(p)
   {
      q=p->next;
      free(p);
      p=q;
   }
}
```

#### 11.求单链表的长度
```c
int  ListLength(LinkList L)
{
    int i=0;
    LinkList p=L->next;
    while(p)
    {
        i++;
        p=p->next;
    }
    return i;
}
```

#### 12.两个单链表的归并
```c
void  MergeList_L(LinkList &La,LinkList &Lb,LinkList &Lc)
{
    LinkList pa,pb,pc;
    pa=La->next;
    pb=Lb->next;
    Lc=pc=La;
    while(pa&&pb)
    {
        if(pa->data<=pb->data)
        {
            pc->next=pa;
            pa=pa->next;
        }
        else
        {
            pc->next=pb;
            pb=pb->next;
        }
        pc=pc->next;
    }
    pc->next=pa?pa:pb;
    free(Lb);
}
```

#### 13.递归实现链表的遍历输出（正序）
```c
void PrintList(LinkList L)
{
    if(L!=NULL)
    {
        printf("%d ",L->data);
        PrintList_1(L->next);
    }
}
```

#### 14.递归实现链表的遍历输出（逆序)
```c
void PrintList(LinkList L)
{
    if(L!=NULL)
    {
        PrintList_2(L->next);
        printf("%d ",L->data);
    }
}
```

#### 15.递归实现链表的逆序
```c
LinkList reverse(LinkList p)
{
    LinkList q,h;
    if(p->next==NULL)
        return p;
    else
    {
        q=p->next;
        h=reverse(q);
        q->next=p;
        p->next=NULL;
        return h;
    }
}
```

#### 16.递归求链表的长度
```c
int ListLength_2(LinkList L)
{
    if(L->next==NULL)
        return 0;
    else
        return 1+ListLength(L->next);
}
```

## 顺序栈

#### 1.顺序栈存储结构
```c
#define STACK_INIT_SIZE 100
#define STACKINCREMENT 10
typedef char SElemType;
typedef struct
{
    SElemType *base;
    SElemType *top;
    int stacksize;
}SqStack;
```

#### 2.顺序栈的初始化
```c
Status InitStack(SqStack &S)
{
    S.base=(SElemType *)malloc(sizeof(SElemType));
    if(!S.base)
        exit(OVERFLOW);
    S.stacksize=0;
    S.top=S.base;
    return OK;
}
```

#### 3.顺序栈的建立
```c
Status InitStack(SqStack &S,int n)
{
    int i;
    S.base=(SElemType *)malloc(sizeof(SElemType)*n);
    if(!S.base)
        exit(OVERFLOW);
    S.stacksize=n;
    for(S.top=S.base,i=0;i<n;S.top++,i++)
        scanf("%c",S.top);
    return OK;
}
```

#### 4.判断栈是否为空
```c
Status StackEmpty(SqStack S)
{
   if(S.top==S.base)
       return TRUE;
    return FALSE;
}
```

#### 5.取栈顶元素
```c
Status GetTop(SqStack S,SElemType &e)
{
    if(S.top==S.base )
        return ERROR;    
    e=*(S.top-1);
    return OK;
}
```

#### 6.元素进栈
```c
Status Push(SqStack &S,SElemType e)
{
    if(S.top-S.base>=S.stacksize)
    {
        SElemType *newbase;
        newbase=(SElemType *)realloc(S.base,
(S.stacksize+STACKINCREMENT)*sizeof(SElemType));
        if(!newbase)
            exit(OVERFLOW);
        S.base=newbase;
        S.top=S.base+S.stacksize;
        S.stacksize +=STACKINCREMENT;
    }
    *(S.top)=e;
    S.top++;
    return OK;
}
```

#### 7.元素出栈
```c
Status Pop(SqStack &S,SElemType &e)
{
    if (S.top==S.base)
        return ERROR;    
    S.top--;
    e=*(S.top);
    return OK;
}
```

#### 8.计算栈中数据元素的个数
```c
int StackLength(SqStack S)
{
    return S.top-S.base;
}
```

#### 9.遍历顺序栈
```c
Status StackTraverse(SqStack S,Status (*Visit)(SElemType e))
{
    SElemType *p;
    if(S.base==S.top)
        return ERROR;
    for(p=S.base;p<S.top;p++)
        Visit(*p);
    printf("\n");
    return OK;
}
```

## 循环队列

#### 1.循环队列存储结构
```c
#define MAXQSIZE 100
typedef char QElemType;
typedef struct
{
    QElemType *base;
    int rear;
    int front;
} SqQueue;
```

#### 2.循环队列的初始化
```c
Status InitQueue(SqQueue &Q)
{
    Q.base=(QElemType *)malloc(sizeof(QElemType)*MAXQSIZE); 
    if(!Q.base)
        exit(OVERFLOW);
    Q.rear=Q.front=0;
    return OK;
}
```

#### 3.循环队列的建立
```c
Status InitQueue(SqQueue &Q,int n)
{
    Q.base=(QElemType *)malloc(sizeof(QElemType)*(n+1)); 
    if(!Q.base)
        exit(OVERFLOW);
    for(Q.front=Q.rear=0;Q.rear<n;Q.rear++)
        scanf("%c",&Q.base[Q.rear]);
    return OK;
}
```

#### 4.判断队列是否为空
```c
Status QueueEmpty(SqQueue Q)
{
    if(Q.front==Q.rear)
        return TRUE;
    return FALSE;
}
```

#### 5.取队首元素
```c
Status GetHead(SqQueue Q,QElemType &e)
{
    if(Q.front==Q.rear)
        return ERROR;
    e=Q.base[Q.front];
    return OK;
}
```

#### 6.元素入队
```c
Status EnQueue(SqQueue &Q,QElemType e)
{
    if((Q.rear+1)%MAXQSIZE==Q.front)
        return ERROR;
    Q.base[Q.rear]=e;
    Q.rear=(Q.rear+1)%MAXQSIZE;
    return OK;
}
```

#### 7.元素出队
```c
Status DeQueue(SqQueue &Q,QElemType &e)
{
    if(Q.front==Q.rear)
        return ERROR;
    e=Q.base[Q.front];
    Q.front=(Q.front+1)%MAXQSIZE;
    return OK;
} 
```

#### 8.计算队列中数据元素的个数
```c
int QueueLength(SqQueue Q)
{
    return (Q.rear-Q.front+MAXQSIZE)%MAXQSIZE;
} 
```

#### 9.遍历循环队列
```c
Status QueueTraverse(SqQueue Q,Status (*Visit)(QElemType e))
{
    int i;
    if(Q.front==Q.rear)
        return ERROR;
    for(i=Q.front;i!=Q.rear;i=(i+1)%MAXQSIZE)
        Visit(Q.base[i]);
    printf("\n");
    return OK;
}
```

## 二叉树

#### 1.二叉树存储结构
```c
typedef char TElemType;
typedef struct BiTNode
{
    TElemType data;    
    struct BiTNode *lchild,*rchild;
}BiTNode ,*BiTree;
```

#### 2.二叉树的创建
```c
Status CreateBiTree(BiTree &T)
{
    char ch;
    scanf("%c",&ch);
    if(ch==' ')
        T=NULL;
    else
    {
        T=(BiTNode *)malloc(sizeof(BiTNode));
        if(!T)
            exit(OVERFLOW);
        T->data = ch;
        CreateBiTree(T->lchild);
        CreateBiTree(T->rchild);
    }
    return OK;
}
```

#### 3.二叉树的遍历（前序）
```c
Status PreOrderTraverse(BiTree T,Status (*Visit)(TElemType))
{
    if(T)
    {
        if(Visit(T->data))    
            if(PreOrderTraverse(T->lchild,Visit))
                if(PreOrderTraverse(T->rchild,Visit))
                    return OK;
        return ERROR;
    }
    else
        return OK;
}
```

#### 4.二叉树的遍历（中序）
```c
Status InOrderTraverse(BiTree T,Status (*Visit)(TElemType))
{
    if(T)
    {
        if(InOrderTraverse(T->lchild,Visit))
            if(Visit(T->data))            
                if(InOrderTraverse(T->rchild,Visit))
                    return OK;
        return ERROR;
    }
    else
        return OK;
}
```

#### 5.二叉树的遍历（后序）
```c
Status PostOrderTraverse(BiTree T,Status (*Visit)(TElemType))
{
    if(T)
    {
        if(PostOrderTraverse(T->lchild,Visit))
            if(PostOrderTraverse(T->rchild,Visit))
                if(Visit(T->data))    
                    return OK;
        return ERROR;
    }
    else
        return OK;
}
```

#### 6.二叉树的遍历（层次）
```c
void LevelOrderTraverse(BiTree T,Status (*Visit)(TElemType))
{
    SqQueue q;
    QElemType a;
    if(T)
    {
       InitQueue(q);
        EnQueue(q,T);
        while(!QueueEmpty(q))
        {
            DeQueue(q,a);
            Visit(a->data);
            if(a->lchild!=NULL)
                EnQueue(q,a->lchild);
            if(a->rchild!=NULL)
                EnQueue(q,a->rchild);
        }
        printf("\n");
    }
}
```

#### 7.求二叉树高度
```c
int TreeDepth(BiTree T)
{
    int depth,depthLeft,depthRight;
    if(!T)
    depth=0;
    else
    {
        depthLeft=TreeDepth(T->lchild);
        depthRight=TreeDepth(T->rchild);
        depth=depthLeft>depthRight?depthLeft:depthRight;
    }
    return depth+1;
}
```

#### 8.交换二叉树的左右子树
```c
void Exchange_Tree(BiTree BT)
{
    BiTree p;
    if(BT)
    {
        Exchange_Tree(BT->lchild);
        Exchange_Tree(BT->rchild);
        p=BT->lchild;
        BT->lchild=BT->rchild;
        BT->rchild=p;
     }
}
```

#### 9.求二叉树的结点个数
```c
void CountNode(BiTree T,int &count)
{
   if(T)
   {
      count++;
      CountNode(T->lchild,count);
      CountNode(T->rchild,count);
   }
}
```

#### 10.求二叉树的叶子数
```c
void CountLeaf(BiTree T,int &count)
{
   
    if(T)
    {
        if((!T->lchild)&&(!T->rchild))
            count++;
        CountLeaf(T->lchild,count);
        CountLeaf(T->rchild,count);
    }
}
```

#### 11.按照目录形式输出二叉树
```c
Status PrintTree(BiTree bt,int nLayer)
{
    int i;
    if(bt!=NULL) 
    {
        PrintTree(bt->lchild,nLayer+1);
        for(i=0;i<nLayer;i++)
            printf(" -");
        printf("%c\n",bt->data);
        PrintTree(bt->rchild,nLayer+1);
    }
    return OK;
}
```

#### 12.二叉树的销毁
```c
void DestroyBiTree(BiTree &T)
{
    if(T)
    {
        DestroyBiTree(T->lchild);
        DestroyBiTree(T->rchild);
        free(T);
        T=NULL;
    }
}
```

## 树

#### 1.树的存储结构
```c
typedef char TElemType;
typedef struct CSNode
{
    TElemType data;
    struct CSNode *firstchild,*nextsibling;
}CSNode,*CSTree;
```

#### 2.求树的深度
```c
int TreeDepth(CSTree &T)
{
    CSTree p;
    int depth,maxdep=0;
    if(!T)
        return 0;
    if(!T->firstchild)
        return 1;
    p=T->firstchild;
    while(p)
    {
        depth=TreeDepth(p);
        if(depth>maxdep)
                    maxdep=depth;
             p=p->nextsibling;
    }
      return maxdep+1;
}
```

#### 3.树的后根遍历
```c
Status InOrderTraverse_CS(CSTree T,Status (*Visit)(TElemType e))
{
    if(T)
    {
        if(InOrderTraverse_CS(T->firstchild,Visit))
            if(Visit(T->data))
                if(InOrderTraverse_CS(T->nextsibling,Visit))                    
                    return OK;
        return ERROR;
    }
    else
        return OK;
}
```

## 查找表

### 顺序表

#### 1.查找表的存储结构
```c
typedef int KeyType;
typedef char InfoType;
#define EQ(a,b) ((a)==(b))
#define LT(a,b) ((a) < (b))
#define LQ(a,b) ((a)=<(b))
typedef struct
{
    KeyType key;
    InfoType otherinfo;
}SElemType;
typedef struct
{
    SElemType *elem;
    int length;
}SSTable;
```

#### 2.顺序查找法
```c
int Search_Seq(SSTable ST,KeyType key)
{
    int i;
    ST.elem[0].key=key;        
    for(i=ST.length;!EQ(ST.elem[i].key,key);i--);
        return i;
}
```

#### 3.折半查找法
```c
int Search_Bin(SSTable ST,KeyType key)
{
    int low=1;
    int high=ST.length;
    int mid;
    while(low<=high)
    {
            mid=(low+high)/2;
        if(EQ(key,ST.elem[mid].key))          
            return mid;
        else if(LT(key,ST.elem[mid].key))
            high=mid-1;     
        else
            low=mid+1;
    }
    return 0;
}
```
### 二叉查找树

### 二叉平衡树

### 哈希表

## 排序表

### 排序表的存储结构
```c
typedef int KeyType;
typedef char InfoType;
#define MAXSIZE 1000
#define EQ(a,b) ((a)==(b))
#define LT(a,b) ((a)<(b))
#define LQ(a,b) ((a)=<(b))
typedef struct 
{
    KeyType key;
   InfoType otherinfo;
}RcdType;
typedef struct
{
    RcdType r[MAXSIZE+1];
    int length;
}SqList;
```

### 插入排序

#### 1.直接插入排序
```c
void InsertionSort(SqList &L) 
{
    int i,j;
    for (i=2;i<=L.length;i++)
        if (L.r[i].key<L.r[i-1].key)
        {
            L.r[0]=L.r[i];
            for(j=i-1; L.r[0].key<L.r[j].key;j--)
    
                L.r[j+1]=L.r[j];
            L.r[j+1]=L.r[0];
        }
}
```

#### 2.折半排序
```c
void BiInsertionSort(SqList &L)
{
    int i,m,low,high;
    for(i=2;i<=L.length;++i)
    {
        L.r[0]=L.r[i];
        low=1;
        high=i-1;
        while(low<=high)
        {
            m=(low+high)/2;
            if(L.r[0].key<L.r[m].key)
                high=m-1;
            else
                low=m+1;
        }
        for(j=i-1;j>=high+1;--j)
            L.r[j+1]=L.r[j];
        L.r[high+1]=L.r[0];
    }
}
```

#### 3.希尔排序
```c
void ShellInsert(SqList &L,int dk)
{
    int i,j;
    for(i=dk+1;i<=L.length;++i)
    {
        if (LT(L.r[i].key,L.r[i-dk].key))
        {
            L.r[0]=L.r[i]; 
            for(j=i-dk; j>0&&LT(L.r[0].key,L.r[j].key);j-=dk)
                L.r[j+dk]=L.r[j];
            L.r[j+dk]=L.r[0];
        }
    }
}
void ShellSort(SqList &L,int dlta[],int t)
{
    int k;
    for(k=0;k<t;++t)
        ShellInsert(L,dlta[k]);
}
```

### 交换排序

#### 1.起泡排序
```c
void BubbleSort(SqList &L)
{
    int i,j;
    int lastExchangeIndex;
    i=L.length;
    RcdType temp;
    while(i>1)
    {
        lastExchangeIndex=1;
        for(j=1;j<i;j++)
                if (L.r[j+1].key<L.r[j].key)
                {
                    temp=L.r[j];
                    L.r[j]=L.r[j+1];
                    L.r[j+1]=temp;
                    lastExchangeIndex=j;
                }
        i=lastExchangeIndex;
    }
}
```

#### 2.快速排序
```c
int Partition(SqList &L,int low,int high)
{
    KeyType pivotkey;
    L.r[0]=L.r[low];
    pivotkey=L.r[low].key;
    while(low<high)
    {
        while(low<high&&L.r[high].key>=pivotkey)
            --high;
        L.r[low]=L.r[high];
        while(low<high&&L.r[low].key<=pivotkey)
            ++low;
        L.r[high]=L.r[low];
    }
	L.r[low]=L.r[0];
	return low;
}
void Qsort(SqList &L,int low,int high)
{
    int pivotloc;
    if(low<high)
    {
        pivotloc=Partition(L,low,high);
        Qsort(L,low,pivotloc-1);
        Qsort(L,pivotloc+1,high);
    }
}
void QuickSort(SqList &L)
{
    Qsort(L,1,L.length); 
}
```

### 选择排序

#### 1.简单选择排序
```c
void SelectSort(SqList &L)
{
    int i,j,k;
    RcdType temp;
    for(i=1;i<L.length;i++)
    {
        j=i;
        for(k=i+1;k<=L.length;k++)
            if (LT(L.r[k].key,L.r[j].key))
                j=k;
        
        if(i!=j)
        {
            temp=L.r[j];
            L.r[j]=L.r[i];
            L.r[i]=temp;
        }
    }
}
```

#### 2.堆排序
```c
void HeapAdjust(SqList &H,int s,int m)
{
    int j;
    RcdType rc=H.r[s];
    for(j=2*s;j<=m;j*=2)
    {
        if(j<m&&LT(H.r[j].key,H.r[j+1].key))
            ++j;
        if(!LT(rc.key,H.r[j].key))
            break;
        H.r[s]=H.r[j];
        s=j;
    }
    H.r[s]=rc;
}
void HeapSort(HeapType &H)
{
    int i;
    RcdType temp;
    for(i=H.length/2;i>0;--i)
        HeapAdjust(H.r,i,H.length);
    for(i=H.length;i>1;--i)
    {
        temp=H.r[1];
        H.r[1]=H.r[i];
        H.r[i]=temp; 
        HeapAdjust(H.r,1,i-1);
    }
}
```

### 归并排序

### 基数排序

## 图

### 存储结构

#### 1.邻接矩阵
```c
#define INFINITY INT_MAX;// 最大值∞
#define MAX_VERTEX_NUM 20;// 最大顶点个数
typedef enum {DG,DN,UDG,UDN} GraphKind;// {有向图,有向网,无向图,无向网}
typedef struct ArcCell
{
    VRType adj;// VRType是顶点关系类型 对无权图,用1或0表示相邻否；对带权图，则为权值类型
    InfoType *info;// 该弧相关信息的指针
}ArcCell,AdjMatrix[MAX_VERTEX_NUM][MAX_VERTEX_NUM];
typedef struct
{
    VertexType vexs[MAX_VERTEX_NUM];// 顶点信息
    AdjMatrix arcs;// 邻接矩阵
    int vexnum,arcnum;// 图的当前顶点数和弧(边)数
    GraphKind kind;// 图的种类标志
}MGraph;
```

#### 2.邻接表
```c
#define MAX_VERTEX_NUM 20
typedef struct ArcNode
{
    int adjvex;// 该弧所指向的顶点的位置
    struct ArcNode *nextarc;// 指向下一条弧的指针
    InfoType *info;// 该弧相关信息的指针
}ArcNode; 
typedef struct VNode
{
    VertexType data;// 顶点信息
    ArcNode *firstarc;// 指向第一条依附该顶点的弧
}AdjList[MAX_VERTEX_NUM];
typedef struct
{
    AdjList vertices;// 顶点数组
    int vexnum,arcnum;// 图的当前顶点数和弧数
    int kind;// 图的种类标志
}ALGraph;
```
#### 3.有向图十字链表

#### 4.无向图的邻接多重表


### 深度优先遍历(DFS)

#### 1.邻接矩阵
```c
void DFS(MGraph G,int v)
{// 从v出发深度优先遍历G
    int j;
    visited[v]=TRUE;
    VisitFunc(G.vexs[v]);
    for(j=0;j<G.numVertexes;j++)
    {
        if (G.arcs[v][j]==1 && !visited[j])  
            DFS(G, j);     
    }
}
```

#### 2.邻接表
```c
void DFS(ALGraph G,int v)
{// 从v出发深度优先遍历G
    visited[v]=TRUE;   
    VisitFunc(G->adjList[v].data);
    p=G.adjList[v].firstarc;
    while(p)
    {
        if(!visited[p->adjvex])  
            DFS(G,p->adjvex);     
        p=p->nextarc;
    }
} 
```
### 广度优先遍历(BFS)


### 构造最小生成树

#### 1.Prim算法
* TE是最小生成树中边的集合；
* 初始令U={u<sub>0</sub>},(u<sub>0</sub>&isin;V),TE=&empty;；
* 在所有u&isin;U,v&isin;V-U的边(u,v)&isin;E中，找一条代价最小的边(u<sub>0</sub>,v<sub>0</sub>)；
* 将(u<sub>0</sub>,v<sub>0</sub>)并入集合TE，同时v<sub>0</sub>并入U；重复上述操作直至U=V为止，则T=(V,{TE})为最小生成树。

#### 2.Kruskal算法
*   初始状态为只有n个顶点而无边的非连通图T=(V,{&empty;})，每个顶点自成一个连通分量；
* 在E中选取代价最小的边，若该边依附的顶点落在T中不同的连通分量上，则将此边加入到T中；否则，舍去此边，选取下一条代价最小的边；
* 依此类推，直至T中所有顶点都在同一连通分量上为止。


### 有向无环图

#### 1.拓扑排序
* 从图中选择一个入度为0的顶点输出；
* 从图中删除该顶点及源自该顶点的所有弧；
* 重复以上两步，直至全部顶点都输出，拓扑排序顺利完成；
* 否则，若剩有入度非0的顶点，说明图中有环，拓扑排序不能进行。

#### 2.关键路径

AOE网
* 路径长度：路径上各活动持续时间之和。
* 关键路径：路径长度最长的路径。
* 关键活动：关键路径上的活动，即这些活动的时间延迟或提前会影响整个工程工期的延迟或提前。


### 最短路径

#### 1.Dijkstra算法
* (1) 初始时,S只包含源点,即S={v},v的距离为0。U包含除v外的其他顶点,U中顶点u距离为边上的权(若v与u有边<v,u>)或∞(若u不是v的出边邻接点)。
* (2) 从U中选取一个距离v最小的顶点k,把k加入S中(该选定的距离就是v到k的最短路径长度)。
* (3) 以k为新考虑的中间点,修改U中各顶点的距离：若从源点v到顶点u(u∈U)的距离(经过顶点k)比原来距离(不经过顶点k)短,则修改顶点u的距离值,修改后的距离值的顶点k的距离加上边<k,u>上的权。
* (4) 重复步骤(2)和(3)直到所有顶点都包含在S中。

#### 2.Floyd算法
* 从图的带权邻接矩阵G.arcs出发，
   假设求顶点V<sub>i</sub>到V<sub>j</sub>的最短路径。如果从V<sub>i</sub>到V<sub>j</sub>有弧，则从V<sub>i</sub>到V<sub>j</sub>存在一条长度为G.arcs[i][j]的路径，但该路径是否一定是最短路径，还需要进行n次试探。
* 第一次，判别（ V<sub>i</sub>, V<sub>0</sub> ）和（ V<sub>0</sub>，V<sub>j</sub>  ），即判别(V<sub>i</sub>, V<sub>0</sub> , V<sub>j</sub>）是否存在，若存在，则比较（ V<sub>i</sub>, V<sub>j</sub> ）和(V<sub>i</sub>, V<sub>0</sub> , V<sub>j</sub>）的长度，取长度较短的为从Vi到Vj的中间顶点序号不大于0的最短路径。
* 第二次，再加一个顶点V<sub>1</sub>，如果(V<sub>i</sub>, … , V1） 和(V<sub>1</sub>, … , V<sub>j</sub>）分别是当前找到的中间顶点序号不大于0的最短路径，那么(V<sub>i</sub>, … , V<sub>1</sub>, … , V<sub>j</sub> ）就有可能是从Vi到V<sub>j</sub>的中间顶点序号不大于1的最短路径。将它和已经得到的从V<sub>i</sub>到Vj之间顶点序号不大于0的最短路径相比较，取较短者为从V<sub>i</sub>到V<sub>j</sub>的中间顶点序号不大于1的最短路径。
* 第三次，再加一个顶点V<sub>2</sub>，继续进行试探。
* ...