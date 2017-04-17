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
        <span class="description">The open source unified CaaS/FaaS platform for 
            <a href="https://docker.com">Docker</a>, batteries included.
        </span>
    </section>

    <ul>
      <li>Host your own high availability cluster or use `cloud.atomiq.io`</li>
      <li><a href="https://github.com/docker/infrakit">Docker Infrakit</a> for self-healing infrastructure</li>
      <li>Use Docker Compose v3 <a href="https://docs.docker.com/compose/compose-file/">stackfiles</a> to deploy your stacks (<a href="https://blog.docker.com/2016/02/containers-as-a-service-caas/">CaaS</a>)</li>
      <li>Support lambda style <a href="https://en.wikipedia.org/wiki/Serverless_computing">serverless</a> tasks (<a href="https://martinfowler.com/articles/serverless.html">FaaS</a>)</li>
      <li>Account management support for users, organizations and teams with role-based access controls</li>
      <li>Logs and metrics realtime filtered feeds and historical query support</li>
      <li><a href="https://www.elastic.co/guide/en/kibana/current/dashboard.html">Kibana dashboard</a> service included</li>
    </ul>

    <p>The current version is 0.9.0. While not recommended for production use quite yet, it's getting close
       (about six weeks away). In the meantime, you can use the current playground hosted at cloud.atomiq.io,
       and you can also host your own cluster. You can even create a full cluster on your own laptop
       with <code>amp cluster create</code> using the CLI.
    </p>
    
    <h2>Getting started</h2>
      <p>
        For getting started and more detailed information, see <a href="https://github.com/appcelerator/amp/blob/master/docs">docs</a>.
      </p>
    
    <h2>Contributing</h2>
      <p>
        If you want to hack on the project, we have a fully containerized toolchain.
        All you need is Docker to build, test, and deploy! We would love for you to get involved,
        so check out <a href="https://github.com/appcelerator/amp/blob/master/project/CONTRIBUTING.md">CONTRIBUTING</a>
        and other docs under <a href="https://github.com/appcelerator/amp/blob/master/project">project</a>.
      </p>
    
    <h2>Community</h2>
      <p>
        If you want to chat with the developers and other members of the community, we've got an
        IRC channel (#atomiq) and you can also join our Slack channel in the next day or so.
      </p>

    <h2>License</h2>

    <p>
      ATOMIQ is licensed under the Apache License, Version 2.0. See <a href="https://github.com/atomiqio/atomiq/blob/master/LICENSE">LICENSE</a>
      for the full license text.
    </p>
</section>


<!--
<section id="announcements">
  {% include announcement/announcement-{{ page.lang }}.md %}
</section>
-->
