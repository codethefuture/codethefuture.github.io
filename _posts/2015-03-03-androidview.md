---
layout: post
title: "AndroidのViewを動的にサイズ変更"
description: ""
category: development
tags: [Android]
---
{% include JB/setup %}

```Java
float newHeight = TypedValue.applyDimension(
	TypedValue.COMPLEX_UNIT_PX,
	getContext().getResources().getDimension(R.dimen.XXX),
	getContext().getResources().getDisplayMetrics()
);
getLayoutParams().height = Math.round(newHeight);
requestLayout();
```
