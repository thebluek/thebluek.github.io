---
---

{% highlight text %}
sudo sudo chown -R www-data: /var/www/
{% endhighlight %}

###npm start without sudo

{% highlight text %}
npm config get prefix
{% endhighlight %}

{% highlight text %}
sudo chown -R $(whoami) $(npm config get prefix)/{lib/node_modules,bin,share}
{% endhighlight %}