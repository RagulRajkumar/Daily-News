<template>
<div class="new" id="new">
  <n-tabs type="line" class="tabs" style="margin-top:10px;">
      <n-tab-pane name="trending" class="tab" tab="Trending in India">
        <India/>
      </n-tab-pane>
      <n-tab-pane name="tech" class="tab" tab="Technology">
        <Technology/>
      </n-tab-pane>
      <n-tab-pane name="sport" class="tab" tab="Sports">
        <Sports/>
      </n-tab-pane>
      <n-tab-pane name="entertainment" class="tab" tab="Entertainment">
        <Entertainment/>
      </n-tab-pane>
      <n-tab-pane name="business" class="tab" tab="Business">
        <Business/>
      </n-tab-pane>
       <n-tab-pane name="health" class="tab" tab="Health">
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
    name:'News',
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
  margin: 10px;
  font-size: 10rem;
}

</style>
