<template>
  <!-- Static navbar -->
  <nav class="navbar navbar-default">
    <div class="container-fluid">
      <div class="navbar-header">
        <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar">
          <span class="sr-only">Toggle navigation</span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
        </button>
        <nuxt-link class="navbar-brand" to="/">Project name</nuxt-link>
      </div>
      <div id="navbar" class="navbar-collapse collapse">
        <ul class="nav navbar-nav">
          <li class="active"><nuxt-link to="/">Home</nuxt-link></li>
          <li><nuxt-link to="/users">Users</nuxt-link></li>
          <li><nuxt-link to="/">Contact</nuxt-link></li>
          <li class="dropdown">
            <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">Dropdown <span class="caret"></span></a>
            <ul class="dropdown-menu">
              <li><nuxt-link to="/">Action</nuxt-link></li>
              <li><nuxt-link to="/">Another action</nuxt-link></li>
              <li><nuxt-link to="/">Something else here</nuxt-link></li>
              <li role="separator" class="divider"></li>
              <li class="dropdown-header">Nav header</li>
              <li><nuxt-link to="/">Separated link</nuxt-link></li>
              <li><nuxt-link to="/">One more separated link</nuxt-link></li>
            </ul>
          </li>
        </ul>
        <ul class="nav navbar-nav navbar-right">
          <li class="active"><a href="./">Default <span class="sr-only">(current)</span></a></li>
          <li><nuxt-link to="/">Static top</nuxt-link></li>
          <li><nuxt-link to="/">Fixed top</nuxt-link></li>
        </ul>
      </div><!--/.nav-collapse -->
    </div><!--/.container-fluid -->
  </nav>
</template>
