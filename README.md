# Document template

A document template made with HTML and CSS *in the making*. 

Demo: http://dev.tmn.io/master/index.pdf

## Printing

There is many ways of getting the HTML and CSS documents into a single "printable" document. 

### Software suggestions
* [Prince](http://princexml.com)
* [WeasyPrint](http://weasyprint.org) (got some restrictions)
* Your favorite web browser (eg. [Opera](http://opera.com/), [Chrome](http://google.com/chrome/)) (got some restrictions)


## Features

#### TOC

Have the TOC-element point to a section ID:

```
<ul class="toc">
  <li><a href="#intro">Introduction</a></li>
</ul>


...


<section class="chapter" id="intro">
  <h1>Introduction</h1>
  <p>Lorem ipsum dolor ...</p>
</section>
```


#### Chapters

```
<div id="content">

  <section class="chapter">
    <h1>Chapter one</h1>
    <p>Content of chapter one</p>
  </section>

  <section class="chapter">
    <h1>Chapter two</h1>
    <p>Content of chapter two</p>
  </section>

</div>
```

#### Sections and subsections

```
<div id="content">

  <section class="chapter">
    <h1>Lorem</section>h1>
    <p>Content</p>

    <section>
      <h1>Ipsum</section>h1>
      <p>Content of subsection</p>

      <section>
        <h1>Dolor</section>h1>
        <p>Content of subsubsection</p>
      </section>
    </section>

  </section>

</div>
```

The chapter title is prefixed with the chapter number. Subsections and subsubsections are prefixed with chapter number and subsection number:

**1  Chapter title**

**1.1  Subsection title**

**1.1.1  Subsubsection titles**

**1.1.2  Subsubsection titles**