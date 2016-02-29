# 2. Structure

## 2.2 CSS

I think in a misxed pf [Atomic Design](http://atomicdesign.bradfrost.com/) and [RSCSS](http://rscss.io/), always think in the styleguides to create concise elements.

### 2.2.1 Tools

My workflow is a constant change , today i'm not use [Kuoto-Swiss](http://kouto-swiss.io/) the powerfull framework to Stylus, but i'll coming soon incorporate him.

- gulp -task runner (with gulp-autoprefixer)
- Stylus - Preprocessor
- jeet.gs - Grid System
- rupture - Breakpoints

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
