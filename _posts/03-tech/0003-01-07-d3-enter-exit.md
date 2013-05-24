---
title: selections
---

{% highlight javascript %}
// select every existing rect element
var rects = d3.selectAll("rect");
rects.attr("fill", "blue"); // fill them all blue
{% endhighlight %}

{% highlight javascript %}
// bind data to a selection with data()
var example = [1,2,3];
rects.data(example);
{% endhighlight %}

{% highlight javascript %}
// create a placeholder selection for data points with no
// matching DOM elements
rects.data(example).enter();
{% endhighlight %}
