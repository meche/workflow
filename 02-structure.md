# 2. Structure

## 2.1 Application

### 2.1.1 The development enviroment

I develop applications front-end using a standard found [here](https://youtu.be/Ma6VVQdvGq4?t=6m6s). Specific Style, one file for each component.

```
+-- dev/
|   +-- css/
|   |   +-- core/ (or generic/)
|   |   |   +-- variables.styl
|   |   |   +-- (...)
|   |   +-- components/
|   |   |   +-- menu.styl
|   |   |   +-- (...)
|   |   +-- styles.styl
|   +-- img/
|   +-- js/
|   |   +-- controllers/
|   |   |   +-- loginCtrl.js
|   |   |   +-- (...)
|   |   +-- directives/
|   |   |   +-- panelDirective.js
|   |   |   +-- (...)
|   |   +-- services/
|   |   |   +-- loginService.js
|   |   |   +-- (...)   
|   |   +-- app.js
|   +-- lib/
|   |   +-- framework/ (Name of the framework)
|   +-- View/
|   |   +-- login.html
|   |   +-- (...)
|   +-- index.html
+-- .gitignore
+-- .travis.yml
+-- gulpfile.js
+-- LICENCE.md
+-- package.json
+-- README.md

```

#### 2.1.1.1 Gulpfile.js

In construction, but i have one exemple [here](https://gist.github.com/meche/0d87318449c58c44b257).

## 2.2 CSS

I think in a misxed pf [Atomic Design](http://atomicdesign.bradfrost.com/) and [RSCSS](http://rscss.io/), always think in the styleguides to create concise elements.

### 2.2.1 Tools

My workflow is a constant change , today i'm not use [Kuoto-Swiss](http://kouto-swiss.io/) the powerfull framework to Stylus, but i'll coming soon incorporate him.

- [gulp](http://gulpjs.com/) -task runner (with gulp-autoprefixer)
- [Stylus](http://stylus-lang.com) - Preprocessor
- [jeet.gs](http://jeet.gs) - Grid System
- [Kuoto-Swiss](http://kouto-swiss.io/) - framework to stylus
- [rupture](https://jenius.github.io/rupture/) - Breakpoints

### 2.2.2 Tree

Basic structure to start projects with stylus

```
+-- application.styl
+-- generic
|   +-- variables.styl
|   +-- mixins.styl
|   +-- resets.styl
|   +-- helpers.styl
+-- components
|   +-- menus.styl
|   +-- cards.styl
|   +-- forms.styl
|   +-- text.styl
|   +-- messages.styl
|   +-- tables.styl
|   +-- (...)
```

### 2.2.3 Patterns

coming soon

## 2.3 HTML

The structure the bolierplate to development one website:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Title Website</title>
    <!--Links CSS-->
</head>
<body>
    <header>
        <h1>Title Website</h1>
    </header>
    <main>
        <p>the content</p>
    </main>
    <footer>
        <small>copyright</small>
    </footer>
    <!-- Scripts -->
</body>

```

### 2.3.1 Syntax

The patterns to visual development and identation

##### 2.3.1.2 I'm use tabs with 4 (four) spaces.

```html
<article class="post-card">
    <h1 class="title">Hello World!</h1>
    <img class="image --responsive" src="" alt="Image post X" >
    <p class="excerpt"></p>    
</article>
```

##### 2.3.1.2 Don't use ```/``` in self-closing elements

```html
<img class="" src="" alt="">
```

##### 2.3.1.3 Double quotes

```html
<article class="post-card">
    (...)
</article>
```

##### 2.3.1.4 Comments

Follow this rule to add comments in HTML.

```html
<!-- Initial comment -->
<!-- Ended comment -->
```

##### 2.3.1.5 Attribute Order

HTML attributes should be in this order for facilitate the reading.

1. `class`
2. `id, name`
3. `data-*`
4. `src, for, type, href`
5. `title, alt`
6. `aria-*, role`

##### 2.3.1.6 Olds IE

For give support a olds Internet Explorer...

```html
<!DOCTYPE html>
<!--[if IE]><![endif]-->
<!--[if IE 7 ]>    <html lang="en" class="ie7">    <![endif]-->
<!--[if IE 8 ]>    <html lang="en" class="ie8">    <![endif]-->
<!--[if IE 9 ]>    <html lang="en" class="ie9">    <![endif]-->
<!--[if (gt IE 9)|!(IE)]><!--><html lang="en"><!--<![endif]-->
<head>
```

### 2.3.2 AMP project

[Go to Docs](https://www.ampproject.org/docs/get_started/about-amp.html).

AMP is a way to build web pages for static content that render fast.

Exemple of file [here](exemples/amp.html).