---
layout: home
title: Atomiq
menu: home
lang: en
redirect_from: "/en/index.html"
---
<section id="home-content">
    {% include header/header-{{ page.lang }}.html %}
    <div id="overlay"></div>

    <section id="description">
        <a href="/" class="express">ATOMIQ</a>

        <span class="description">Microservices for
        <a href='https://nodejs.org/en/'>Node.js</a>
        </span>
    </section>

    <div id="install-command">
      $ npm install -g yo<br>
      $ npm install -g generator-atomiq<br>
      $ yo atomiq
    </div>
</section>

<section id="intro">

  <div id="boxes" class="clearfix">
      <div id="microservices">
          <h3>Microservices</h3> Atomiq is a generator and lightweight
          library to facilitate writing microservices for container
          environments. It is not a framework and there is no "magic".<br><br>
          Atomiq does offer a straightforward directory-based routing
          convention on top of <a href='http://expressjs.com'>Express</a>
          based on ES6 classes that you can exploit if you desire.
      </div>

      <div id="babel">
          <h3>Babel</h3> Atomiq uses ES6 and <code>async/await</code>, and provides support for automatically transpiling your source files with
          <a href="https://babeljs.io/">Babel</a>.
      </div>

      <div id="docker">
          <h3>Docker</h3> Microservices are intended primarily
          for container environments. Support for running in
          <a href="https://docker.com">Docker</a>
          containers and for debugging with Node Inspector is built in.
      </div>

  </div>

</section>


<!--
<section id="announcements">
  {% include announcement/announcement-{{ page.lang }}.md %}
</section>
-->
