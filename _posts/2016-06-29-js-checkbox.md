---
layout: post
title:  Javascript 统计checkbox数量

date:   2016-06-29 15:08:00 +0800
categories: document
tag: javascript
---

* content
{:toc}



### 1 统计checkbox数量

```javascript

jQuery:

$("input:checkbox:checked").length;




Dom:

var inputElems = document.getElementsByTagName("input");

var count = 0;

for (var i=0; i<inputElems.length; i++)

{

    if (inputElems[i].type === "checkbox" && inputElems[i].checked === true)

    {

        count++;

    }

}

```
