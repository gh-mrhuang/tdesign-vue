<template>
  <div class="demo-slider">
    <div class="vertical-marks-block">
      <t-slider v-model="value1" @change="change" :layout="layout" vertical :show-tooltip="true" :marks="marks1" />
    </div>

    <div class="vertical-marks-block">
      <t-slider v-model="value2" :layout="layout" vertical range :show-tooltip="true" :marks="marks2" />
    </div>
  </div>
</template>
<script lang="jsx">
export default {
  data() {
    return {
      value1: 12,
      value2: [30, 70],
      layout: 'vertical',
      marks1: {
        0: '0°C',
        20: '20°C',
        40: '40°C',
        60: '60°C',
        80: <span style="color: #0052d9">80°C</span>,
        100: <span style="color: #0052d9">100°C</span>,
      },
      marks2: {
        0: '0°C',
        20: '20°C',
        40: '40°C',
        60: '60°C',
        80: <span style="color: #0052d9">80°C</span>,
        100: <span style="color: #0052d9">100°C</span>,
      },
    };
  },
  methods: {
    change(value) {
      console.log('change value', value);
    },
  },
};
</script>
<style>
.vertical-marks-block {
  display: inline-block;
  padding: 30px 70px;
  height: 300px;
}
</style>
