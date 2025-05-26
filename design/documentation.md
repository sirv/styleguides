# Documentation design
Some documentation design guidelines

### References:
[How to write Sirv's documentation](/content/documentation.html)

## Screenshots

<details>
  <summary>Click to open</summary>
Font used for screenshots: ShadowsIntoLight Sirv font.ttf
[font](https://3.basecamp.com/3562099/blobs/84ed75d4-fc1c-11e7-8449-ecf4bbcece28/download/ShadowsIntoLight%20Sirv%20font.ttf)

Arrows used for screenshots:

![alt text](https://sirv.sirv.com/blue-arrow-1.png?w=60)

    https://sirv.sirv.com/blue-arrow-1.png


----------
![alt text](https://sirv.sirv.com/blue-arrow-2.png?w=40)

    https://sirv.sirv.com/blue-arrow-2.png

----------
![alt text](https://sirv.sirv.com/blue-arrow-3.png?w=60)

    https://sirv.sirv.com/blue-arrow-3.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/a_blue.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/a_blue.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/a.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/a.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/b_blue.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/b_blue.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/b.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/b.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/c_blue.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/c_blue.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/c.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/c.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/d_blue.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/d_blue.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/d.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/d.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/e_blue.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/e_blue.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/e.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/e.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/f_blue.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/f_blue.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/f.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/f.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/g_blue.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/g_blue.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/g.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/g.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/h_blue.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/h_blue.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/h.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/h.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/k_blue.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/k_blue.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/k.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/k.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/l_blue.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/l_blue.png
----------

![alt text](https://sirv.sirv.com/website/screenshots/arrows/l.png?w=60)

    https://sirv.sirv.com/website/screenshots/arrows/l.png


### Colours of arrows/text in screenshots:


**Blue**: <span style="color:#317bba">#317bba</span>

**Red**: <span style="color:#c42734">#c42734</span>

Example screenshots:

![alt text](https://sirv-cdn.sirv.com/Style%20Guide/screenshot1.png)



![alt text](https://sirv-cdn.sirv.com/Style%20Guide/screenshot2.png)

Screenshots should be saved using a unique and descriptive name (with suitable keywords) and uploaded to this folder of the sirv account:

[https://my.sirv.com/#/browse/website/screenshots](https://my.sirv.com/#/browse/website/screenshots)

Lists in the documentation should be numerated in  and with proper HTML markup (ol tag):
1. Create an account.
2. Upload the images.
3. Create a spin.
etc.

</details>

## Grid
half, third, fourth classes

example:

```html
<div class="row">
  <div class="half">
    <p>wwwww</p>
  </div>
</div>
```


## Shortcodes
`[smv]` for inserting the latest version of Sirv Media Viewer's script.

`[taxposts tax_id="47"]` for insterting all posts from a certain category.

`[table][/table]` - adaptive table

`[pre][/pre]` - for code with with copy functionality
`.code-inline` class - apply to a paragraph or a span for nice inline code highlight.

`[blockquote type="awesome" cite="John Smith" content="Content ...."]`
`[/blockquote]` - for blockquote

`[sc_fs_multi_faq  headline-0="em" question-0="How does it work?" answer-0="Somehow" headline-1="em"  question-1="something something?" answer-1="no."  html="true" ]` - for FAQ. Each question needs 3 elements: headline tag, question and answer. all numbered (first starts with an 0 ( question-0  etc.)
 html="true" - this will render the questions on the page (if false - it'll just generate json-ld structured data. 
headline-0="em" can be headline-0="h4" for a heading instead of the cursive.
Also important - using links and html in shortcodes - just use single quotes. 

*Notes*

`[notes title="Not type" content="new not types notes"]` without type

`[notes type="warning" title="Warning" content="new warning notes"]` warning type

`[notes type="important" title="Important" content="new important notes"]` important type

You can use this code to achieve a two column look
```html
<div class="category-section">
[taxposts tax_id="56"]
</div>
```
## Inline code or whatever block
```<span class="code-inline">loop</span>```

## Responsive video embeds (YouTube, Vimeo, etc.)
Use this CSS:
```html
<style>
.videoWrapper {
	position: relative;
	padding-bottom: 56.25%; /* 16:9 */
	padding-top: 25px;
	height: 0;
}
.videoWrapper iframe {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
}
</style>
```
Wrap the video in the container
```html
<div class="videoWrapper">
<iframe width="560" height="305" src="https://www.youtube.com/embed/_NODkWcHeW0?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>
```

## Ordered list for proper SEO

Use

```html
<ol class="mainlist">
<li>Item 1</li>
<li>item 2 etc...</li>
</ol>
```
