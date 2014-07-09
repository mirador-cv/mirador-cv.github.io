---
layout: post
title:  "Python & Ruby Support"
date:   2014-07-09 15:36:10
categories: api clients
---

We've created official clients for the Mirador realtime image moderation API in Python and Ruby. Of course, they're both open-source!

With our packages on PyPi and Rubygems, it's super easy to get started:

```
pip install mirador
```

To classify an image (just replace with your API key):

{% highlight python %}
>>> from mirador import MiradorClient
>>> mc = MiradorClient('your_key_here')
>>> mc.classify_urls('http://demo.mirador.im/test/nsfw.jpg')
[<MiradorResult: http://demo.mirador.im/test/nsfw.jpg; safe: False; value: 0.999999502312/>]
>>>
{% endhighlight %}

To read the source and the full documentation, see our github repos:

### python: [mirador-py](http://mirador-cv.github.io/mirador-py)
### ruby: [mirador-rb](http://mirador-cv.github.io/mirador-rb)

As always, feel free to shoot us an email at support@mirador.im with any problems or questions!
