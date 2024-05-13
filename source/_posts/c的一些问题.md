---
title: c的一些问题
date: 2024-04-28 19:09:20
description: 集合。如果太长了就另开界面。
index_img:
tags:
categories: 
- knowledge
archive:
---

### 实现输入整型数据串后敲回车结束输入

例子：

```
void main(){
    int* p=NULL;
    int n=1;
    
    p = (int*)realloc(p,n*sizeof(int));
    if(p==NULL)
        exit(1);
    for(int i = 0;;i++){
        p = (int*)realloc(p,(++n)*sizeof(int));
        scanf("%d",p+i);
        if(getchar()=='\n')break;
    }
    //可能是因为scanf在读取时会自动跳过空格读取下一个数+scanf读取完后顺位的空格or回车被getchar读取。综合下来实现了只要敲回车就能输入数据的功能。
    
    for(i = 0;i<n-1;i++)  printf("%d  ",*(p+i));

}
```
