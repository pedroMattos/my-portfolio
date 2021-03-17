<template>
  <div id="backend">
    <h3 class="centralizer white">Backend</h3>
    <v-chart class="chart" :option="option" />
  </div>
</template>

<script>
import { use } from "echarts/core";
import { CanvasRenderer } from "echarts/renderers";
import { RadarChart } from "echarts/charts";
import {
  TitleComponent,
  TooltipComponent,
  LegendComponent,
} from "echarts/components";
import VChart, { THEME_KEY } from "vue-echarts";
import { ref, defineComponent } from "vue";
use([
  CanvasRenderer,
  RadarChart,
  TitleComponent,
  TooltipComponent,
  LegendComponent,
]);

export default {
  name: "graph-skills-back",
  components: {
    VChart,
  },
  data() {
    return {
      option: {
        tooltip: {},
        radar: {
          // shape: 'circle',
          name: {
            textStyle: {
              color: "#fff",
              backgroundColor: "#D94169",
              borderRadius: 3,
              padding: [3, 5],
            },
          },
          indicator: [
            { name: "Express", max: 100 },
            { name: "Websockets", max: 100 },
            { name: "NodeJs", max: 100 },
            { name: "Python", max: 100 },
            { name: "PHP", max: 100 },
            { name: "API Rest", max: 100 },
          ],
        },
        series: [
          {
            name: "Backend Skills",
            type: "radar",
            data: [
              {
                value: [80, 70, 80, 80, 85, 80],
                name: "Backend Skills",
              },
            ],
            itemStyle: {
              color: "#D94169",
            },
          },
        ],
      },
    };
  },
};
</script>
