---
layout: post
title:  "How to use rvm and gemset"
date:   2015-05-22 10:43:52
categories: ruby
---

#### **RVM**
Show all ruby versions in your system.
{% highlight ruby %}
~$ rvm list
{% endhighlight %}

Install ruby, example: "install ruby 2.1.5".
{% highlight ruby %}
~$ rvm install 2.1.5
{% endhighlight %}

How to use determinate version of ruby, example: "use ruby-2.1.5".
{% highlight ruby %}
~$ rvm use 2.1.5
{% endhighlight %}

Set default ruby versions.
{% highlight ruby %}
~$ rvm use 2.2.2 --default
{% endhighlight %}

#### **GEMSET**
To list the full directory path for the current gemset:
{% highlight ruby %}
~$ rvm gemdir
{% endhighlight %}

To list all named gemsets for the current ruby interpreter.
{% highlight ruby %}
~$ rvm gemset list
{% endhighlight %}

**Creating gemsets**

Gemsets must be created before being used. To create a new gemset for the current ruby, do this:
{% highlight ruby %}
~$ rvm gemset create teddy
{% endhighlight %}

You can also create multiple gemsets in a single command.
{% highlight ruby %}
~$ rvm gemset create teddy roise
{% endhighlight %}

Alternatively, if you prefer the shorthand syntax offered by rvm use, employ the --create option like so:
{% highlight ruby %}
~$ rvm use 2.1.5@teddy --create
{% endhighlight %}

**Using Gemsets**

Before you can use a gemset, you must first create it.

To use a gemset:
{% highlight ruby %}
~$ rvm gemset use teddy
{% endhighlight %}

You can switch to a gemset as you start to use a ruby, by appending @gemsetname to the end of the ruby selector string:
{% highlight ruby %}
~$ rvm use 2.1.5@teddy
{% endhighlight %}

**Emptying Gemsets**

If you empty a gemset, rvm will prompt you for confirmation. This action removes all gems installed in the gemset.

{% highlight ruby %}
~$ rvm gemset use teddy
~$ rvm gemset empty teddy
{% endhighlight %}

To skip confirmation, pass the --force flag:
{% highlight ruby %}
~$ rvm gemset use teddy
~$ rvm --force gemset empty teddy
{% endhighlight %}

**Deleting Gemsets**

When you delete a gemset, rvm will prompt you to confirm the deletion.
{% highlight ruby %}
~$ rvm gemset use teddy
~$ rvm gemset delete teddy
{% endhighlight %}

To skip confirmation, pass the --force flag:
{% highlight ruby %}
~$ rvm gemset use teddy
~$ rvm --force gemset delete teddy
{% endhighlight %}

<br /><br />
happy code..!
