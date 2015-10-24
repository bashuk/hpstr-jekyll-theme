---
layout: page
title: HPSTR cheatsheet
image:
  #background:
  #feature:
  #credit:
  #creditlink:
permalink: /cs/
---

## Markdown cheatsheet
<https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet>

## Images

{% capture images %}
    http://upload.wikimedia.org/wikipedia/en/2/24/Lenna.png     
    https://upload.wikimedia.org/wikipedia/commons/5/5f/Utah_teapot_simple_2.png
    /images/cheatsheet/1.png
{% endcapture %} {% include gallery images=images caption="Test images" cols=3 %}

Code:

{% highlight jinja %}
{% raw %}
{% capture images %}
    http://upload.wikimedia.org/wikipedia/en/2/24/Lenna.png     
    https://upload.wikimedia.org/wikipedia/commons/5/5f/Utah_teapot_simple_2.png
    /images/PM5544_with_non-PAL_signals.png
{% endcapture %} {% include gallery images=images caption="Test images" cols=3 %}
{% endraw %}
{% endhighlight %}

## Videos

<iframe width="560" height="315"
src="//www.youtube.com/embed/C0DPdy98e4c"
frameborder="0"> </iframe>

Code:

{% highlight html %}
<iframe width="560" height="315"
src="//www.youtube.com/embed/C0DPdy98e4c"
frameborder="0"> </iframe>
{% endhighlight %}

Pay attention to the space between the `<iframe>` tags.

## Code embedding

{% highlight cpp %}
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, world!" << endl;
    return 0;
}
{% endhighlight %}

Code:
{% highlight jinja %}
{% raw %}
{% highlight python %}
print "Hello, world!"
{% endhighlight %}
{% endraw %}
{% endhighlight %}

## Custom buttons

<div markdown="0">
    <a href="#" class="btn">Primary Button</a>
    <a href="#" class="btn btn-success">Success Button</a>
    <a href="#" class="btn btn-warning">Warning Button</a>
    <a href="#" class="btn btn-danger">Danger Button</a>
    <a href="#" class="btn btn-info">Info Button</a>
</div>

Code:

{% highlight html %}
<div markdown="0">
    <a href="#" class="btn">Primary Button</a>
    <a href="#" class="btn btn-success">Success Button</a>
    <a href="#" class="btn btn-warning">Warning Button</a>
    <a href="#" class="btn btn-danger">Danger Button</a>
    <a href="#" class="btn btn-info">Info Button</a>
</div>
{% endhighlight %}
