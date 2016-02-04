# Hypermark!

Markdown is Hypertext.

Inspirational, fast, reversible,
extendable, and filterable.

ॐ


## Current Usage

```pycon
>>> import hypermark

>>> content = "# fuck yea\nhttp://github.com"

>>> d = hypermark.text(content)
'<HyperText 7c7706acb8>'

>>> d.links
['http://github.com']

>>> d.hash
u'03a392ef91826a3506fcc54a4e1fa7b022688ec42bc4d53b4c36a8b6f8058606'

>>> print(d.html)
<h1>fuck yea</h1>
<p><a href="http://github.com">http://github.com</a></p>
```

## Filters!

```pycon
>>> d.filters('bleach').html
u'&lt;h1&gt;fuck yea&lt;/h1&gt;\n&lt;p&gt;http://github.com&lt;/p&gt;'
```

## Vision (Work in Progress)

Feature ideas:

1. link extraction
1. diff generation
1. sha generation
1. md->html, html->md
1. header transposing
1. stripping?
1. targets for headers

This could, potentially, contain a lot of the basic functionality of wikis.org
itself — would help explain the core concepts to the world, perhaps.
