---
layout: post
title:  "Welcome to Jekyll!"
date:   2020-02-09 17:10:23 +0100
categories: jekyll update
include_mathjax: true
---

<script src="/assets/demos/UnityWebAsm/TemplateData/UnityProgress.js"></script>
<script src="/assets/demos/UnityWebAsm/Build/UnityLoader.js"></script>
<script>
  var unityInstance = UnityLoader.instantiate("unityContainer", "/assets/demos/UnityWebAsm/Build/Builds.json", {onProgress: UnityProgress});
</script>

You’ll find this post in your `template <typename T>` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

{% include aside.html content="This is an aside! I'm here to let you know about something you might find interesting" %}

Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

{% include aside.html content="This is a second aside that was created automatically with an include!" %}

Jekyll also offers powerful support for code snippets:

```ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
```

```cpp
namespace reg_helper
{
  template <typename T>
  inline int call(void(*f)())
  {
    // This is dumb hacky code
    static const int s = [&f]() {
      f();
      return 0;
    }();
    return s;
  }
}
```

Here's some maths, which renders really nicely,

<div>When \(a \ne 0\), there are two solutions to \(ax^2 + bx + c = 0\) and they are
  \[x = {-b \pm \sqrt{b^2-4ac} \over 2a}.\]</div>

Here's something even more intimidating, the friendly Christoffel symbols,

<div>
\[(\nabla_X Y)^k = X^i (\nabla_i Y)^k =
           X^i \left( \frac{\partial Y^k}{\partial x^i} + \Gamma_{im}^k Y^m \right)\]
</div>

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/

You’ll find this post in your `template <typename T>` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

```ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
```


Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].


We're also able to run WebGL interactive windows on our web pages

<div class="webgl-content">
  <div id="unityContainer" style="width: 660px; height: 400px"></div>
  <div class="footer">
    <div class="webgl-logo"></div>
    <div class="fullscreen" onclick="unityInstance.SetFullscreen(1)"></div>
    <div class="title">ExplorableExplanations</div>
  </div>
</div>


[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/

