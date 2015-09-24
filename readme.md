<h1>paper-vert-tabs</h1>

<h3>Vertical paper tabs for Polymer 1.0</h3>

These tabs work just like regular <a href="https://elements.polymer-project.org/elements/paper-tabs">Paper Tabs</a> except of course they are aligned vertically!

```html
<link rel="import" href="../bower_components/paper-vert-tabs/paper-vert-tabs.html">

<paper-vert-tabs id="tabs" selected="0">
	<paper-tab>Tab 1</paper-tab>
	<paper-tab>Tab 2</paper-tab>
</paper-vert-tabs>
```
```javascript
var tabs = document.getElementById('tabs');
var pages = document.getElementsByTagName('neon-animated-pages')[0];
//change the page based on tab selection
tabs.addEventListener('iron-select', function() {
	pages.select(tabs.selected);
}
```

<h3>Attributes</h3>
<ul>
<li><strong>align-left</strong>: (Boolean) If true, the selection bar will align to the left side of the tabs. Default: false.</li>
<li><strong>no-bar</strong>: (Boolean) If true, the selection bar will not be shown. Default: false.</li>
<li><strong>no-slide</strong>: (Boolean) If true, the slide effect for the selection bar will be disabled. Default: false.</li>
<li><strong>no-ink</strong>: (Boolean) If true, the ink ripple effect is disabled. Default: false.</li>
<li>Other attributes from <a href="https://elements.polymer-project.org/elements/paper-tabs">Paper Tabs</a> should work as well.</li>
<li><strong>selected</strong>: (Number) Gets or sets the selected element. The default is to use the index of the item. For example:</li>
</ul>


