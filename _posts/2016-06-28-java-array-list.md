---
layout: post
title:  Java, convert List <--> Array 
date:   2016-06-28 15:08:00 +0800
categories: document
tag: Java
---

* content
{:toc}



### 1. convert List to Array

```java

Foo[] array = list.toArray(new Foo[list.size()]);

or:

Foo[] array = new Foo[list.size()];
list.toArray(array); // fill the array

```



### 2. Array to List

```java

dataList[];

new ArrayList<>(Arrays.asList(dataList) );

```
