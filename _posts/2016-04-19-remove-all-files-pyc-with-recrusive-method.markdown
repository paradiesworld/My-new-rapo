---
title: Remove all files .pyc with recrusive method
date: 2016-04-19 07:39:34 Z
categories:
- python
- bash
layout: post
---

This method simple but important. Example in your project dir is like this:

{% highlight ruby %}
project_dir/
           __init__.py
           __init__.pyc
           something.py
           something.pyc
           ...
           core/
               __init__.py
               __init__.pyc
               build.py
               build.pyc
{% endhighlight %}

Deleting the `.pyc` files one by one would be spending a lot of time. and you will be bored. There is sample how to handle it.

```
$ find your_dir -name *.pyc -delete
```

OR, if you work inside current directory.

```
$ find . -name *.pyc -delete
```