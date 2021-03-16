  <template>
  <div id="app">
    <message>Hello There</message>
    <message>Hello There</message>
    <message
      ><template>Hello There</template>
      <counter></counter>
    </message>
    <message>
      <ajax-axios-request></ajax-axios-request>
    </message>
  </div>
</template>

<script>
/* import HelloWorld from './components/HelloWorld.vue' */
import Message from "./components/Message";
import Counter from "./components/Counter";
import AjaxAxiosRequest from "./components/AjaxAxiosRequest.vue";

export default {
  name: "App",
  components: {
    Message,
    Counter,
    AjaxAxiosRequest,
  },
  data() {
    return {};
  },
};
</script>

<style>
#app {
}
</style>
