<template>
  <div class="hello">
    <div class="wrapper">
      <h1 contenteditable data-heading="Alison Yoon">Alison Yoon</h1>
    </div>
    <h1>{{ msg }}</h1>

    <p>
      Shortly after she joined the team, the new interface and usability of the
      new application got positive feedbacks from stakeholders, internal team,
      and customers. Her work is appreciated overall, and she continues to work
      together with development team, engaging stakeholders and users to
      improve, create the product that provides great experience.
    </p>
    <p>
      Here, she designs cloud based web application. It’s a dashboard that deals
      with large, complex data that provides filtering, data modeling.
    </p>
    <p>
      You can see the challenges and process of her work
      <router-link to="/about">here.</router-link>
    </p>
    <p>
      Her previous work was at
      <a href="roundee.io">roundee.io</a> where she worked as UI/UX designer.
      She created design system for the brand, redesigned the website, carried
      market research, user interviews, UX workshops with internal team,
      delivered production level prototype with UI development.
    </p>
    <p>
      She worked as a freelance web designer working with clients. She worked as
      an independent graphic designer after finishing her degree in fashion.
    </p>
    <!-- <h3>Installed CLI Plugins</h3>
    <ul>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel"
          target="_blank"
          rel="noopener"
          >babel</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint"
          target="_blank"
          rel="noopener"
          >eslint</a
        >
      </li>
    </ul>-->
    <h3>Essential Links</h3>
    <ul>
      <li>
        <a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a>
      </li>
      <li>
        <a href="https://forum.vuejs.org" target="_blank" rel="noopener"
          >Forum</a
        >
      </li>
      <li>
        <a href="https://chat.vuejs.org" target="_blank" rel="noopener"
          >Community Chat</a
        >
      </li>
      <li>
        <a href="https://twitter.com/vuejs" target="_blank" rel="noopener"
          >Twitter</a
        >
      </li>
      <li>
        <a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a>
      </li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li>
        <a href="https://router.vuejs.org" target="_blank" rel="noopener"
          >vue-router</a
        >
      </li>
      <li>
        <a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a>
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-devtools#vue-devtools"
          target="_blank"
          rel="noopener"
          >vue-devtools</a
        >
      </li>
      <li>
        <a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener"
          >vue-loader</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/awesome-vue"
          target="_blank"
          rel="noopener"
          >awesome-vue</a
        >
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

$bg: #e6e2df;

html,
body {
  height: 100%;
}

body {
  background: linear-gradient(45deg, $bg 80%, #c2c1bd 100%);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.wrapper {
  width: 100%;
  font-family: 'Source Code Pro', monospace;
  margin: 0 auto;
  position: relative;
  top: 100px;
  height: 180px;

  h1 {
    text-transform: uppercase;
    transform: translate(-50%, -50%) skew(10deg) rotate(-10deg);
    font-size: 5vw;
    top: -10%;
    left: 20%;
    margin: 0;
    position: absolute;
    text-rendering: optimizeLegibility;
    font-weight: 900;
    color: rgba(#ff9eb1, 0.5);
    text-shadow: 1px 4px 6px $bg, 0 0 0 #66303a, 1px 4px 6px $bg;
    white-space: nowrap;

    &:before {
      content: attr(data-heading);
      position: absolute;
      left: -17px;
      top: -4.8%;
      overflow: hidden;
      width: 100%;
      height: 50%;
      color: #fbf7f4;
      transform: translate(1.6vw, 0) skew(-13deg) scale(1, 1.2);
      z-index: 2;
      text-shadow: 2px -1px 6px rgba(0, 0, 0, 0.2);
    }

    &:after {
      content: attr(data-heading);
      position: absolute;
      left: 0;
      top: 0;
      overflow: hidden;
      width: 100%;
      height: 100%;
      z-index: 1;
      color: #d3cfcc;
      transform: translate(0vw, 0) skew(13deg) scale(1, 0.8);
      clip-path: polygon(0 50%, 100% 50%, 100% 100%, 0% 100%);
      text-shadow: 2px -1px 6px rgba(0, 0, 0, 0.3);
    }
  }
}
</style>
