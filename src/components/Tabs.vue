<template>
<div class="new" id="new">
  <button name="trending" tab="Trending in India" ></button>
  <n-tabs type="line" style="margin-top:10px;">
      <n-tab-pane name="trending" tab="Trending in India">
        <India/>
      </n-tab-pane>
      <n-tab-pane name="tech" tab="Technology">
        <Technology/>
      </n-tab-pane>
      <n-tab-pane name="sport" tab="Sports">
        <Sports/>
      </n-tab-pane>
      <n-tab-pane name="entertainment" tab="Entertainment">
        <Entertainment/>
      </n-tab-pane>
      <n-tab-pane name="business" tab="Business">
        <Business/>
      </n-tab-pane>
       <n-tab-pane name="health" tab="Health">
        <Health/>
      </n-tab-pane>
    </n-tabs>
</div>
</template>

<script>
import India from './India.vue';
import Technology from './Technology.vue';
import Sports from './Sports.vue';
import Entertainment from './Entertainment.vue';
import Business from './Business.vue';
import Health from './Health.vue';
import { NTabs } from 'naive-ui'
import { NTabPane } from 'naive-ui'

export default {
    name:'Tabs',
  components: {
      NTabs,
      NTabPane,
      India,
      Technology,
      Sports,
      Entertainment,
      Business,
      Health

    }
};

</script>

<style>
#new {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  display:flex;
  flex-wrap: wrap;
  justify-content: center;
  text-align: center;
  align-items: center;
  background-color: #ffffff;  
  overflow-y: scroll;
}
</style>
