---
---

{% highlight bash %}
git branch
{% endhighlight %}

*feature/fragment
master

{% highlight bash %}
git branch -D feature/fragment
{% endhighlight %}

*master

{% highlight bash %}
git branch feature/readme
git branch
{% endhighlight %}

feature/readme
* master

{% highlight bash %}
git branch
{% endhighlight %}

*feature/readme
master

{% highlight bash %}
vi README.md
{% endhighlight %}

{% highlight bash %}
git status
{% endhighlight %}

README.md

{% highlight bash %}
git branch
{% endhighlight %}

feature/readme
* master

{% highlight bash %}
git checkout feature/readme
git branch
{% endhighlight %}

* feature/readme
master

{% highlight bash %}
git status
{% endhighlight %}

README.md

{% highlight bash %}
git add .
git commit -m “Add README.md”
git remote -v
{% endhighlight %}

origin https://github.com/jangho/MyRepository.git (fetch)
origin https://github.com/jangho/MyRepository.git (push)
upstream https://github.com/thebluek/MyRepository.git (fetch)
upstream https://github.com/thebluek/MyRepository.git(push)

{% highlight bash %}
git push origin feature/readme
{% endhighlight %}

{% highlight bash %}
git branch
{% endhighlight %}

* feature/readme
master

{% highlight bash %}
git checkout master
git pull upstream master
git branch -D feature/readme
{% endhighlight %}
