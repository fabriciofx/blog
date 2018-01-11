---
layout: post
title: "Educational Aspect of Static Analysis"
date: 2018-01-16
place: Moscow, Russia
tags: quality
description: |
  ...
keywords:
  - static analysis
  - teaching by static analysis
  - code auto-formatting
  - auto-formatting
  - java static analysis
image: /images/2018/01/
jb_picture:
  caption:
---

[Very often](https://github.com/yegor256/cactoos/issues/544)
new programmers who join our projects ask us whether we
have auto-formatting instruments to make Java code look exactly
how [Qulice]({% pst 2014/aug/2014-08-13-strict-code-quality-control %})
expects&mdash;the static analyzer we use. I always reply that having
such an automated code polisher would only be harmful and won't help
the project and its members improve and grow. Here is why I think so.

<!--more-->

{% jb_picture_body %}

Static analysis, the way we do it in a combination with
[read-only master branch]({% pst 2014/jul/2014-07-21-read-only-master-branch %}),
is a fully automated uncompromising review of your pull request, mostly
intended to to spot code formatting mistakes. Say, we want Java code in
our entire repository look like this:

{% highlight java %}
final class Doc {
  private final File file;
  public void remove() {
    if (this.file.exists()) {
      this.file.delete();
    }
  }
}
{% endhighlight %}

However, you refactor it, as part of a bigger task, and submit a pull request:

{% highlight java %}
class Doc {
  private File f;
  public void remove()
  {
    if (f.exists())
      f.delete();
  }
}
{% endhighlight %}

For some of you this may not be a big difference, since both code snippets
compile without issues and work exactly the same way. However, for us,
repository maintainers, it's a big deal. We do want our classes to be
always `final`, we want them to be immutable (all attributes should be `final`),
we want to prefix all attribute references with `this.`, and we want the
code to be formatted the same way, since we believe that the uniformity
of the code seriously increases its maintainability.

Of course, we can create a tool, which you will just ask to re-format
the code, to make it look like we want. But in this case you will
never _learn_ what the project wants from you and _why_.

You will not know the reasoning behind our rules. You will never think about them.
You will not really care about them. But they are not only about formatting
of spaces and brackets. There are [over 900]({% pst 2014/jul/2014-07-21-read-only-master-branch %})
of them in [Qulice](http://www.qulice.com) and some of
them were designed especially for the object-oriented philosophy
[we](http://www.elegantobjects.org) are preaching.

Thus, simply put, we don't want you to go through the static analysis phase easily.
We want you to suffer in order to learn.
