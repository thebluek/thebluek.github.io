---
---

### HTML
{% highlight html %}
<div id="root"></div>
{% endhighlight %}

### JS

{% highlight javascript %}

class Codelab extends React.Component {
  render() {
    let text = 'Hi I am codelab';
    let style = {
      backgroundColor: 'aqua'
    }
    return(
      <div style={style}>{/* comment */}{text}</div>
    );
  }
}

class App extends React.Component {
  render() {
    return (
      <Codelab/>
    );
  }
}

ReactDOM.render(<App/>,document.getElementById('root'));

{% endhighlight %}

### Result
{% highlight text %}
Codelab
{% endhighlight %}