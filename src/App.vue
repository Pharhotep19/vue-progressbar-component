<template>
  <div id="app">
    <div class="my-5 container">
      <header class="my-3 clearfix">
        <ul class="nav float-right">
          <li class="nav-item">
            <a class="nav-link" href="https://github.com/EvodiaAut/vue-progressbar-component" target="_blank">Github</a>
          </li>
        </ul>
        <h1 class="text-muted">vue-progressbar-component</h1>
        <p class="lead">[<a href="https://www.smashingmagazine.com/2016/12/gpu-animation-doing-it-right/" target="_blank">CSS GPU Animation</a>] Simple progressbar for vuejs</p>
        <p class="d-flex flex-wrap">
          <a href="https://www.npmjs.com/package/vue-progressbar-component" target="_blank">
            <img class="m-1" src="https://img.shields.io/npm/v/vue-progressbar-component.svg?style=for-the-badge" alt="vue-progressbar-component npm">
          </a>
          <a href="https://github.com/EvodiaAut/vue-progressbar-component/blob/master/LICENSE.md" target="_blank">
            <img class="m-1" src="https://img.shields.io/github/license/mashape/apistatus.svg?style=for-the-badge" alt="vue-progressbar-component license">
          </a>
          <a href="https://www.npmjs.com/package/vue-progressbar-component" target="_blank">
            <img class="m-1" src="https://img.shields.io/npm/dt/vue-progressbar-component.svg?style=for-the-badge" alt="vue-progressbar-component npm">
          </a>
        </p>
      </header>
      <hr>
      <main role="main">
        <div class="row my-5">
          <div class="col-md-6 my-3">
            <h4>Simple progressbar to 77%</h4>
            <p>Set a value <code>:value="77"</code></p>
            <progress-bar :value="77"></progress-bar>
            <h4 class="my-3">Change scale to Y</h4>
            <p>Set <code>:value="88" scale="Y" origin="bottom"</code></p>
            <progress-bar style="height:350px" :value="88" scale="Y" origin="bottom"></progress-bar>
          </div>
          <div class="col-md-6 my-3">
            <h4>Transform Origin</h4>
            <p>Use <code>:value="95" origin="right"</code> for change transform origin</p>
            <progress-bar :value="95" origin="right"></progress-bar>
            <p class="my-3"><code>:value="90" origin="center"</code></p>
            <progress-bar :value="90" origin="center"></progress-bar>
          </div>
        </div>
      </main>
    </div>
  </div>
</template>

<script>
import ProgressBar from './components/ProgressBar'

export default {
  name: 'app',
  components: {
    ProgressBar
  }
}
</script>

<style lang="scss">
  /*
    ProgressBar
  */
  @import "scss/progressbar";

  /*
    Bootstrap
  */
  @import "../node_modules/bootstrap/scss/functions";
  @import "../node_modules/bootstrap/scss/variables";
  @import "../node_modules/bootstrap/scss/mixins";
  // @import "../node_modules/bootstrap/scss/root";
  // @import "../node_modules/bootstrap/scss/print";
  @import "../node_modules/bootstrap/scss/reboot";
  @import "../node_modules/bootstrap/scss/type";
  @import "../node_modules/bootstrap/scss/images";
  @import "../node_modules/bootstrap/scss/code";
  @import "../node_modules/bootstrap/scss/grid";
  // @import "../node_modules/bootstrap/scss/tables";
  // @import "../node_modules/bootstrap/scss/forms";
  // @import "../node_modules/bootstrap/scss/buttons";
  // @import "../node_modules/bootstrap/scss/transitions";
  // @import "../node_modules/bootstrap/scss/dropdown";
  // @import "../node_modules/bootstrap/scss/button-group";
  // @import "../node_modules/bootstrap/scss/input-group";
  // @import "../node_modules/bootstrap/scss/custom-forms";
  @import "../node_modules/bootstrap/scss/nav";
  // @import "../node_modules/bootstrap/scss/navbar";
  // @import "../node_modules/bootstrap/scss/card";
  // @import "../node_modules/bootstrap/scss/breadcrumb";
  // @import "../node_modules/bootstrap/scss/pagination";
  @import "../node_modules/bootstrap/scss/badge";
  @import "../node_modules/bootstrap/scss/jumbotron";
  // @import "../node_modules/bootstrap/scss/alert";
  // @import "../node_modules/bootstrap/scss/progress";
  // @import "../node_modules/bootstrap/scss/media";
  // @import "../node_modules/bootstrap/scss/list-group";
  // @import "../node_modules/bootstrap/scss/close";
  // @import "../node_modules/bootstrap/scss/modal";
  // @import "../node_modules/bootstrap/scss/tooltip";
  // @import "../node_modules/bootstrap/scss/popover";
  // @import "../node_modules/bootstrap/scss/carousel";
  @import "../node_modules/bootstrap/scss/utilities";
</style>
