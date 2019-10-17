<template>
  <div class="social-container">
    <ul>
      <li class="hvr-float">
        <a href="https://github.com/niconj" target="_blank">
          <img src="../assets/github.svg">
        </a>
      </li>
      <li class="hvr-float">
        <a href="https://www.linkedin.com/in/nicolasjeremias/" target="_blank">
          <img src="../assets/linkedin.svg">
        </a>
      </li>
      <li class="hvr-float">
        <a href="https://www.instagram.com/nico_nj/" target="_blank">
          <img src="../assets/instagram.svg">
        </a>
      </li>
      <li class="hvr-float">
        <a href="mailto:jeremias.nicolas@gmail.com?Subject=hello!">
          <img src="../assets/gmail.svg">
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Social-Contact',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  img {
    width:30px;
  }

  @media (max-width: 768px) {
    img {
      width:25px;
    }
  }

  /* Float */
  .hvr-float {
    display: inline-block;
    vertical-align: middle;
    -webkit-transform: perspective(1px) translateZ(0);
    transform: perspective(1px) translateZ(0);
    box-shadow: 0 0 1px rgba(0, 0, 0, 0);
    -webkit-transition-duration: 0.3s;
    transition-duration: 0.3s;
    -webkit-transition-property: transform;
    transition-property: transform;
    -webkit-transition-timing-function: ease-out;
    transition-timing-function: ease-out;
  }
  .hvr-float:hover, .hvr-float:focus, .hvr-float:active {
    -webkit-transform: translateY(-5px);
    transform: translateY(-5px);
  }
</style>
