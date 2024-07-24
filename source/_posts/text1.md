---
title: text1
index_img: https://raw.githubusercontent.com/shuangyanshan/image/main/img/freecompress-%E3%80%8A-%E6%B0%B4-%E6%BC%AB-%E9%87%91-%E5%B1%B1-%E3%80%8B_100285573.jpeg 
date: 2024-03-25 22:27:41
categories:
tags:
hide: true
---

### 测试

#### hhh

<!-- more -->

---

<u>emmm</u>

_hhh_

![](https://raw.githubusercontent.com/shuangyanshan/image/main/img/942016582!figure_large.jpg)

{% fold info "折叠块的标题"%}

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

{% endfold %}

# latex

\documentclass[a4paper,12pt]{article}

\begin{document}

A sentence of text.

\end{document}

$2+3 =5$
$$2+3 = 5$$
