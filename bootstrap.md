# Boostrap 4

---

## Intro

- Bootstrap 4 is the latest version of the widely popular front-end framework, [Bootstrap](http://getbootstrap.com/).
- Bootstrap 4 has a lot of new exciting features and capabilities that make building responsive designs even easier than before. The biggest add-on is that it is heavily built on Flexbox. <!-- .element: class="fragment fade-up" -->

<aside class="footnote">
![](https://www.google.com/s2/favicons?domain=medium.freecodecamp.org) [Bootstrap 4: Everything You Need to Know – freeCodeCamp](https://medium.freecodecamp.org/bootstrap-4-everything-you-need-to-know-c750991f6784)
</aside>

---

## Reasons to learn Bootstrap

1. Fast Prototyping <!-- .element: class="fragment fade-up" -->
1. Responsive Web Design <!-- .element: class="fragment fade-up" -->
1. Old Codebase <!-- .element: class="fragment fade-up" -->

<aside class="footnote">
![](https://www.google.com/s2/favicons?domain=medium.freecodecamp.org) [Bootstrap 4: Everything You Need to Know – freeCodeCamp](https://medium.freecodecamp.org/bootstrap-4-everything-you-need-to-know-c750991f6784)
</aside>

---

## Getting started

Use the [Starter Template](https://getbootstrap.com/docs/4.1/getting-started/introduction/#starter-template)

--

### Starter Template

```html
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.1/css/bootstrap.min.css" integrity="sha384-WskhaSGFgHYWDcbwN70/dfYBj47jz9qbsMId/iRN3ewGhXQFZCSftd1LZCfmhktB" crossorigin="anonymous">

    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.1/js/bootstrap.min.js" integrity="sha384-smHYKdLADwkXOn1EmN1qk/HfnUcbVRZyYmZ4qpPea6sjB/pTJ0euyQp0Mk8ck+5T" crossorigin="anonymous"></script>
  </body>
</html>
```

--

### Falling back from CDN to local

```html
<!-- CSS -->
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.1/css/bootstrap.min.css" integrity="sha384-WskhaSGFgHYWDcbwN70/dfYBj47jz9qbsMId/iRN3ewGhXQFZCSftd1LZCfmhktB" crossorigin="anonymous">

<!-- JavaScript -->
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.1/js/bootstrap.min.js" integrity="sha384-smHYKdLADwkXOn1EmN1qk/HfnUcbVRZyYmZ4qpPea6sjB/pTJ0euyQp0Mk8ck+5T" crossorigin="anonymous"></script>

<!-- Local fallback -->
<script>
  if (!$.fn.modal) {
    document.write('<script src="/js/bootstrap.min.js"></script>');
    document.write('<link rel="stylesheet" href="/css/bootstrap.min.css">');
  }
</script>
```

<aside class="footnote">
![](https://www.google.com/s2/favicons?domain=www.hanselman.com) [CDNs fail, but your scripts don't have to - fallback from CDN to local jQuery - Scott Hanselman](https://www.hanselman.com/blog/CDNsFailButYourScriptsDontHaveToFallbackFromCDNToLocalJQuery.aspx)
</aside>

--

### Package managers

- NPM
- YARN
- Bower
- Webpack <sup>*</sup>

---

## Reboot

- Builds upon `Normalize`
- Additional styling is done only with classes.

<aside class="footnote">
![](https://www.google.com/s2/favicons?domain=getbootstrap.com) [Reboot · Bootstrap](https://getbootstrap.com/docs/4.1/content/reboot/)
</aside>

---

## Basic Styles

--

### Typography

- `rem`s vc `em`s
- avoid `margin-top`
- inherit when possible
- `border-box` sizing
- native font stacks
- special styles

--

### Classes

- `container`
- `h1` … `h6`
- `display-1` … `display-4`
- `lead`

--

### Alignment Utilities

- `text-justify`
- `text-nowrap`
- `text(-<xx>)-<pos>`
  - xx: `sm` (576px), `md` (768px), `lg` (992px), `xl` (1200px)
  - pos: `left`, `center`, `right`

--

### Capitalization

- `text-lowercase`
- `text-uppercase`
- `text-capitalize`

--

### Text Styles

- `font-weight-bold`
- `font-weight-normal`
- `font-italic`

--

### Lists

- `lists-unstyled`
- `list-inline`
- `list-inline-item`

--

### Blockquotes

- `blockquote`
- `blockquote-footer`
- `blockquote-reverse`

--

### Text Colors

- `text-<class>`
  - class: `primary`, `secondary`, `success`, `danger`, `warning`, `info`, `light`, `dark`, `white`

--

### Background Colors

- `bg-<class>`
  - class: `primary`, `secondary`, `success`, `danger`, `warning`, `info`, `light`, `dark`, `white`
- `bg-faded`

--

### Basic Images

- `img-fluid`
- `rounded`, `rounded-<dir>`
  - dir: `top`, `right`, `bottom`, `left`, `circle`, `0`
- `img-thumbnail`

--

### Aligning Images

- `float-left`, `float-right`
- `text-center` on container
- `mx-auto`

<aside class="footnote">
![](https://www.google.com/s2/favicons?domain=getbootstrap.com) [Spacing · Bootstrap](https://getbootstrap.com/docs/4.1/utilities/spacing/)
</aside>

--

### Figures

- `figure` on `<figure>`
- `figure-img` on `<img>`
- `figure-caption` on `<figcaption>`

--

### CSS variables

```css
:root {
    --pink: #eee;
    --danger: #ddd;
    --breakpoint-xs
    --font-family-sans-serif
    --font-samily-monospace
}
```

---

## Layout

--

### Overview

- responsive 12-column
- Flexbox based

--

### Structure

- containers
  - rows
    - columns

--

### Containers

- `container`
- `container-fluid`
  - 15px padding
  - 576px, 576px, 768px, 992pz, 1200px

--

### Columns

- 12 Column Grid
- Columns can span
- `col(-<bp>)-<num>`
  - bp: `sm` (576px), `md` (768px), `lg` (992px), `xl` (1200px)
  - num: `1` &hellip; `12`

--

### Offsets

- `offset-<bp>-<num>`
  - bp: `sm` (576px), `md` (768px), `lg` (992px), `xl` (1200px)
  - num: `1` &hellip; `12`

--

### Nested columns

- `row` inside column
- Creates 12-col grid
- Use same classes

--

### Custom order

- `order-(<bp>)-ord`
  - bp: `sm` (576px), `md` (768px), `lg` (992px), `xl` (1200px)
  - num: `1` &hellip; `12`
- Need to set it for every column

--

### Vertical Allignment

- Use in rows
- `align-items-<aln>`
- aln: `start`, `center`, `end`

--

### Individual Alignment

- Use in cols
- `align-self-<aln>`
  - aln: `start`, `center`, `end`

--

### Horizonal Alignment

- Use in rows
- Need col width
- `justify-content(-<bp>)-<aln>`
  - bp: `sm` (576px), `md` (768px), `lg` (992px), `xl` (1200px)
  - aln: `start`, `center`, `end`, `around`, `between`

--

### Position

- `fixed-top`
- `fixed-bottom`
- `sticky-top`
  - `position: sticky`
  - lacks support

--

### Basic Display

- Mimics CSS
- `d(-<bp>)-<typ>`
  - bp: `sm` (576px), `md` (768px), `lg` (992px), `xl` (1200px)
  - typ: `none`, `inline`, `inline-block`, `block`, `table`, `table-row`, `table-cell`, `flex`, `inline-flex`

--

### Print Display

- `d-print-<typ>`
  - typ: `none`, `inline`, `inline-block`, `block`, `table`, `table-row`, `table-cell`, `flex`, `inline-flex`
  - e.g. `d-none d-print-block`

--

### Flexbox container

- Basic Flex Container
  - `d(-<bp>)-<inline)-flex` &amp; &hellip;
- Direction
  - `flex(-<bp>)(-<dir>)(-reverse)`
    - dir: `row` , `column`

--

### Alignment

- Justify
  - `justify-content(-<bp>)-<aln>`
    - aln: `start`, `center`, `end`, `around`, `between`
- Wrap
  - `flex(-<bp>)-wrp(-reverse)`
    - wrp: `wrap`, `nowrap`
- Vertical Alignment
  - `align-content(-<bp>)-<alg>`
    - alg: `start`, `center`, `end`, `around`, `between`, `stretch`

--

### Flex elements

- `order-(<bp>)-ord`
  - ord: `1` &hellip; `12`
- `align-self-<aln>`
  - aln: `start`, `center`, `end`, `baseline`, `stretch` (default)

--

### Floating elements

- `float(-<bp>)-<sid>`
  - sid: `left`, `right`, `none`

--

### Margin and padding

- `<pro>(<sid)(-<bp>)-<siz>`
  - pro: `m` (margin), `p` (padding)
  - sid: `t`, `r`, `b`, `l`, `x`, `y`
  - siz: `0` &hellip; `5`, `auto`
    - 3 => 1 rem

--

### Visibility

- `invisible`, `visible`
- `d(-<bp>)-<typ>`
  - typ: `none`, `inline`, `inline-block`, `block`, `table`, `table-row`, `table-cell`, `flex`, `inline-flex`

--

### Sizing utilities

- `<siz>(-<amt>)`
  - siz: `w`, `h`, `mw` (max) , `mh` (max)
  - amt: `25`, `50`, `75`, `100` (percent)

--

### Borders

- `border(-<sid>)(-<color>)(-0)`
  - sid: `top`, `right`, `bottom`, `left`
  - color: `primary`, `secondary`, `success`, `danger`, `warning`, `info`, `light`, `dark`, `white`
- `rounded(-<sid>)(-circle|-0)`

---

## Navs &amp; Navbar

--

### Basic Nav Classes

- `nav` or `ul.nav`
- `nav-item` (on `li` or `a`)
  - `nav-link`

--

### Link Options

- `active`, `disabled`
- `nav-pills`, `nav-tabs`

--

### Alignment

- `justify-content-center`, `justify-content-end`
- `nav-fill` (variable width), `nav-justified` (fixed width)
- `flex-column` (on container to force vertical stack)
  - `flex-column flex-sm-row`

--

### Basic Example

```html
<nav class="navbar bg-dark navbar-dark navbar-expand-sm">
  <div class="container">
      <div class="navbar-nav">
          <a class="nav-item nav-link active" href="#">Home</a>
          <a class="nav-item nav-link" href="#">Mission</a>
          <a class="nav-item nav-link" href="#">Services</a>
          <a class="nav-item nav-link" href="#">Staff</a>
          <a class="nav-item nav-link" href="#">Testimonials</a>
      </div>
  </div>
</nav>
```

--

### Branding &amp; text

```html
<nav class="navbar bg-dark navbar-dark navbar-expand-sm">
  <div class="container">
      <h2 class="navbar-band d-none d-sm-inline-block" href="/">My Company</h2>
      <div class="navbar-nav">
          <a class="nav-item nav-link active" href="#">Home</a>
          <a class="nav-item nav-link" href="#">Mission</a>
          <a class="nav-item nav-link" href="#">Services</a>
          <a class="nav-item nav-link" href="#">Staff</a>
          <a class="nav-item nav-link" href="#">Testimonials</a>
      </div>
  </div>
  <span class="navbar-text d-none d-sm-inline-block">Some text</span>
</nav>
```

--

### Dropdown

```html
<nav id="navbar-site" class="navbar bg-dark navbar-dark navbar-expand-sm">
    <div class="container">
        <div class="navbar-nav ml-sm-auto">
            <a class="nav-item nav-link active" href="#">Home</a>
            <a class="nav-item nav-link" href="#">Mission</a>
            <div class="dropdown show">
                <a class="btn btn-secondary dropdown-toggle" href="#" role="button" id="dropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                    Dropdown link
                </a>
                <div class="dropdown-menu" aria-labelledby="dropdownMenuLink">
                    <a class="dropdown-item" href="#">Action</a>
                    <a class="dropdown-item" href="#">Another action</a>
                    <a class="dropdown-item" href="#">Something else here</a>
                </div>
                </div>
            <a class="nav-item nav-link" href="#">Staff</a>
            <a class="nav-item nav-link" href="#">Testimonials</a>
        </div>
    </div>
    <span class="navbar-text d-none d-sm-inline-block">Some text</span>
</nav>
```

--

### Form elements

```html
<nav class="navbar navbar-dark bg-dark navbar-expand-sm">
  <div class="container">
    <ul class="navbar-nav">
      <li class="nav-item"><a class="nav-link" href="#mission">Mission</a></li>
      <li class="nav-item"><a class="nav-link" href="#services">Services</a></li>
      <li class="nav-item"><a class="nav-link" href="#staff">Staff</a></li>
      <li class="nav-item"><a class="nav-link" href="#testimonials">Testimonials</a></li>
    </ul><!-- navbar-nav -->
    <form class="form-inline">
      <input class="form-control mr-2" type="text" placeholder="Search">
      <button class="btn btn-outline-light" type="submit">Go</button>
    </form>
  </div><!-- container -->
</nav>
```

--

### Collapsible content

```html
<nav class="navbar navbar-dark bg-dark navbar-expand-sm">
  <div class="container">

    <button class="navbar-toggler" type="button"
      data-toggle="collapse" data-target="#myTogglerNav"
      aria-controls="myTogglerNav"
      aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <a href="#" class="navbar-brand">Wisdom Pet Medicine</a>

    <div class="collapse navbar-collapse" id="myTogglerNav">
      <div class="navbar-nav">
        <a class="nav-item nav-link active" href="#">Home</a>
        <a class="nav-item nav-link" href="#">Mission</a>
        <a class="nav-item nav-link" href="#">Services</a>
        <a class="nav-item nav-link" href="#">Staff</a>
        <a class="nav-item nav-link" href="#">Testimonials</a>
      </div><!-- navbar -->
    </div><!-- collapse -->

  </div><!-- container -->
</nav><!-- nav -->
```

---

## Style elements

--

### Button

- `btn` &amp;
  - `btn-<siz>`
    - siz: `sm`, `lg`
- on `<a>`, `<button>`, `<input>`

--

### Buttons Colors

- `btn` &amp;
  - `btn-<color>`, `btn-outline-<color>`
  - `btn-block` full width
  - `acive`, `disabled`

--

### Button groups

- `btn-group`
- `btn-group-vertical`
- `btn-toolbar`

--

### Example

```html
<div class="btn-toolbar" aria-label="All Pets">
<div class="btn-group  btn-group-lg mb-2 mr-2" aria-label="Common Pets">
  <button type="button" class="btn btn-primary active">Cat</button>
  <button type="button" class="btn btn-primary">Dog</button>
  <button type="button" class="btn btn-primary">Fish</button>
  <button type="button" class="btn btn-primary">Bird</button>
</div>

<div class="btn-group btn-group-sm mb-2" aria-label="Exotic Pets">
  <button type="button" class="btn btn-primary">Amphibian</button>
  <button type="button" class="btn btn-primary active">Reptile</button>
  <button type="button" class="btn btn-primary">Other</button>
</div>
</div>

<div class="btn-group btn-group-vertical" aria-label="Exotic Pets">
  <button type="button" class="btn btn-primary">Amphibian</button>
  <button type="button" class="btn btn-primary active">Reptile</button>
  <button type="button" class="btn btn-primary">Other</button>
</div>
```

--

### Badges

- `badge`, `badge-pill` &amp;
  - `badge-<color>`
- usually on `<span>`

--

### Progress bar

```html
<div class="progress">
    <div class="progress-bar" role="progressbar" aria-value-now="73%" aria-value-min="0"  aria-value-max="100%" style="width:73%">73%</div>
    </div>
<div class="progress">
    <div class="progress-bar bg-success progress-bar-striped" style="width:85%"></div>
    </div>
<div class="progress">
    <div class="progress-bar bg-info" style="width:15%"></div>
    <div class="progress-bar bg-warning" style="width:30%"></div>
    </div>
<div class="progress">
    <div class="progress-bar bg-warning" style="width:15%"></div>
    </div>
<div class="progress">
    <div class="progress-bar bg-danger" style="width:15%"></div>
</div>
```

--

### List groups

```html
<ul class="list-group mb-3">
  <li class="list-group-item active">Grooming</li>
  <li class="list-group-item list-group-item-action">General Health</li>
  <li class="list-group-item list-group-item-action d-flex justify-content-between align-items-center">Nutrition
    <span class="badge badge-primary badge-pill">12</span></li>
  <li class="list-group-item list-group-item-action">Pest Control</li>
  <li class="list-group-item list-group-item-action">Vaccinations</li>
</ul>

<div class="mb-3 list-group">
  <a class="list-group-item list-group-item-action active" href="#">Grooming</a>
  <a class="list-group-item list-group-item-action list-group-item-success" href="#">General Health</a>
  <a class="list-group-item list-group-item-action list-group-item-info" href="#">Nutrition</a>
  <a class="list-group-item list-group-item-action list-group-item-warning" href="#">Pest Control</a>
  <a class="list-group-item list-group-item-action list-group-item-danger" href="#">Vaccinations</a>
</div>

<div class="list-group mb-3">
  <button class="list-group-item list-group-item-action active" type="button">Grooming </button>
  <button class="list-group-item list-group-item-action" type="button">General Health</button>
  <button class="list-group-item list-group-item-action" type="button">Nutrition</button>
  <button class="list-group-item list-group-item-action" type="button">Pest Control</button>
  <button class="list-group-item list-group-item-action" type="button">Vaccinations</button>
</div>
```

--

### Breadcrumbs

```html
<ol class="breadcrumb">
  <li class="breadcrumb-item"><a href="#">Home</a></li>
  <li class="breadcrumb-item"><a href="#">Exotic Pets</a></li>
  <li class="breadcrumb-item active">Nutrition</li>
</ol>

<nav class="breadcrumb">
  <a class="breadcrumb-item" href="#">Home</a>
  <a class="breadcrumb-item" href="#">Exotic Pets</a>
  <span class="breadcrumb-item active">Nutrition</span>
</nav>
```

---

## Form Styles

--

### Basic

```html
<form>

  <fieldset class="form-group">
    <legend>Owner Info</legend>

    <div class="form-group">
      <label class="form-control-label" for="ownername">Owner name</label>
      <input class="form-control" type="text" id="ownername" placeholder="Your Name">
    </div><!-- form-group -->

    <div class="form-group">
      <label class="form-control-label" for="owneremail">Email address</label>
      <input class="form-control" type="email" id="owneremail" aria-describedby="emailHelp" placeholder="Enter email">
      <small class="form-text text-muted" id="emailHelp">We'll never share your email</small>
    </div><!-- form-group -->

  </fieldset><!-- fieldset -->
  <fieldset class="form-group">

    <legend>Pet Info</legend>

    <div class="form-group">
      <label class="form-control-label" for="petname">Pet name</label>
      <input class="form-control" type="text" id="petname" placeholder="Your Pet's name">
    </div><!-- form-group -->

    <div class="form-group">
      <label class="form-control-label" for="pettype">Pet type</label>
      <select class="form-control" id="pettype">
        <option>Choose</option>
        <option value="cat">Dog</option>
        <option value="cat">Cat</option>
        <option value="bird">Other</option>
      </select>
    </div><!-- form-group -->

    <div class="form-group">
      <label class="form-control-label" for="reasonforvisit">Reason for today's visit</label>
      <textarea class="form-control" id="reasonforvisit" rows="3"></textarea>
    </div><!-- form-group -->


  </fieldset><!-- fieldset -->
  <button class="btn btn-primary" type="submit">Submit</button>
</form>
```

--

### Checkboxes &amp; radios

```html
<form>

  <fieldset class="form-group">
    <legend>Owner Info</legend>

    <div class="form-group">
      <label class="form-control-label" for="ownername">Owner name</label>
      <input class="form-control" type="text" id="ownername" placeholder="Your Name">
    </div><!-- form-group -->

    <div class="form-group">
      <label class="form-control-label" for="owneremail">Email address</label>
      <input class="form-control" type="email" id="owneremail" aria-describedby="emailHelp" placeholder="Enter email">
      <small class="form-text text-muted" id="emailHelp">We'll never share your email</small>
    </div><!-- form-group -->

  </fieldset><!-- fieldset -->
  <fieldset class="form-group">

    <legend>Pet Info</legend>

    <div class="form-group">
      <label class="form-control-label" for="petname">Pet name</label>
      <input class="form-control" type="text" id="petname" placeholder="Your Pet's name">
    </div><!-- form-group -->

    <div class="form-group">
      <label class="form-control-label" for="pettype">Pet type</label>
      <select class="form-control" id="pettype">
        <option>Choose</option>
        <option value="cat">Dog</option>
        <option value="cat">Cat</option>
        <option value="bird">Other</option>
      </select>
    </div><!-- form-group -->

    <div class="form-group">
      <label class="form-control-label" for="reasonforvisit">Reason for today's visit</label>
      <textarea class="form-control" id="reasonforvisit" rows="3"></textarea>
    </div><!-- form-group -->
  </fieldset><!-- fieldset -->

  <fieldset class="form-group">

    <legend>Pet Medical Data</legend>

    <div class="form-group">
      <label class="d-block">Has your pet been spayed or neutered?</label>

      <div class="form-check form-check-inline">
        <label class="form-check-label">
          <input class="form-check-input" type="radio" name="spayneut" value="yes" checked> Yes
        </label>
      </div><!-- form-check -->

      <div class="form-check form-check-inline">
        <label class="form-check-label">
          <input class="form-check-input" type="radio" name="spayneut" value="no"> No
        </label>
      </div><!-- form-check -->

    </div><!-- form-group -->

    <div class="form-group">
      <label>Has the pet had any of the following in the past 30 days</label>

      <div class="form-check">
        <label class="form-check-label">
          <input class="form-check-input" type="checkbox"> Abdominal pain
        </label>
      </div><!-- form-check -->

      <div class="form-check">
        <label class="form-check-label">
          <input class="form-check-input" type="checkbox"> Lack of appetite
        </label>
      </div><!-- form-check -->

      <div class="form-check">
        <label class="form-check-label">
          <input class="form-check-input" type="checkbox"> Weakness
        </label>
      </div><!-- form-check -->
    </div><!-- form-group -->

  </fieldset><!-- form-group -->

  <button class="btn btn-primary" type="submit">Submit</button>
</form>
```

---

## Resources / Next steps

- ![](https://www.google.com/s2/favicons?domain=medium.freecodecamp.org) [Learn Bootstrap 4 in 5 minutes – freeCodeCamp](https://medium.freecodecamp.org/learn-bootstrap-4-in-5-minutes-da94728efe41)
- ![](https://www.google.com/s2/favicons?domain=medium.freecodecamp.org) [Bootstrap 4: Everything You Need to Know – freeCodeCamp](https://medium.freecodecamp.org/bootstrap-4-everything-you-need-to-know-c750991f6784)
- ![](https://www.google.com/s2/favicons?domain=scrimba.com) [Learn Bootstrap 4 for free | Scrimba.com](https://scrimba.com/g/gbootstrap4?utm_source=Scrimba+main&utm_campaign=41dc47aa8e-EMAIL_CAMPAIGN_2018_01_25&utm_medium=email&utm_term=0_1475ca4552-41dc47aa8e-92449423)
