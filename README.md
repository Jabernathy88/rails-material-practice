## Dev notes

```
rails new ghostmapmedia2 --database=postgresql -T --no-rdoc --no-ri

gem 'materialize-sass', '~> 1.0.0'

bundle

rename to: app/assets/stylesheets/application.scss

Css:
@import "materialize";

@import "materialize/components/color-variables";
$primary-color: color("blue", "lighten-2") !default;
$secondary-color: color("yellow", "base") !default;
@import 'materialize';

Js:
//= require materialize

Html:
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet"> 

rails g controller pages index

<!-- Dropdown Structure -->
<ul id="dropdown1" class="dropdown-content">
  <li><a href="#!">one</a></li>
  <li><a href="#!">two</a></li>
  <li class="divider"></li>
  <li><a href="#!">three</a></li>
</ul>
<nav>
  <div class="nav-wrapper">
    <a href="#!" class="brand-logo">Logo</a>
    <ul class="right hide-on-med-and-down">
      <li><a href="sass.html">Sass</a></li>
      <li><a href="badges.html">Components</a></li>
      <!-- Dropdown Trigger -->
      <li><a class="dropdown-trigger" href="#!" data-target="dropdown1">Dropdown<i class="material-icons right">arrow_drop_down</i></a></li>
    </ul>
  </div>
</nav>

<script src="https://code.jquery.com/jquery-1.9.1.min.js"></script>

<script>
  $( document ).ready(function() {
    $(".dropdown-trigger").dropdown();
    console.log( "document loaded" );
  });
</script>
```