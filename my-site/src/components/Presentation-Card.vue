<template>
  <div class="card-container">
    <div class="card">
      <h1>
        Hi! I'm <span>Nico.</span>
      </h1>
      <h2>I'm a web developer who loves to design and build great experiences</h2>

      <section class="bio">
        <p>I've been building software for more than 6 years for a wide variety of clients.<br>
        You can check some of my personal projects on <a class="hvr-underline-from-center" href="https://github.com/niconj" target="_blank">Github</a> and my work experience in <a class="hvr-underline-from-center" href="https://www.linkedin.com/in/nicolasjeremias/" target="_blank">LinkedIn</a></p>

        <p>During my free time I enjoy <a class="hvr-underline-from-center" href="https://ar.pinterest.com/nicolsjeremas/diy/" target="_blank">woodworking</a>, stand up comedy and trekking. <br><br>
        Do you want to get in touch? <br>
        <a class="hvr-underline-from-center" href="mailto:jeremias.nicolas@gmail.com?Subject=hello!">Send me a message!</a></p>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Presentation-Card',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card-container {
  margin: 5% 25%;
}

@media (max-width: 768px) {
  .card-container {
    margin: 10% 15%;
  }
}

.card {
  text-align: left;
}

h1 span {
  font-size: 1.3em;
  font-family: 'Indie Flower', cursive;
  color: #3B568C;
}

.bio {
  margin-top: 3em;
}

.bio a {
  font-weight: bold;
  text-decoration: none;
  color: inherit;
}

h1, h2 {
  margin: 0;
}

/* Underline From Center */
.hvr-underline-from-center {
  display: inline-block;
  vertical-align: middle;
  -webkit-transform: perspective(1px) translateZ(0);
  transform: perspective(1px) translateZ(0);
  box-shadow: 0 0 1px rgba(0, 0, 0, 0);
  position: relative;
  overflow: hidden;
}
.hvr-underline-from-center:before {
  content: "";
  position: absolute;
  z-index: -1;
  left: 51%;
  right: 51%;
  bottom: 0;
  /* background: #2098D1; */
  background: #3B568C;
  height: 4px;
  -webkit-transition-property: left, right;
  transition-property: left, right;
  -webkit-transition-duration: 0.3s;
  transition-duration: 0.3s;
  -webkit-transition-timing-function: ease-out;
  transition-timing-function: ease-out;
}
.hvr-underline-from-center:hover:before, .hvr-underline-from-center:focus:before, .hvr-underline-from-center:active:before {
  left: 0;
  right: 0;
}
</style>
