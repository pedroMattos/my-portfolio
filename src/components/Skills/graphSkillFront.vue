<template>
  <div id="frontend">
    <h3 class="centralizer white">Frontend</h3>
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
  name: "graph-skills-front",
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
            { name: "Web Scrapping", max: 100 },
            { name: "CSS/SCSS", max: 100 },
            { name: "JavaScript", max: 100 },
            { name: "UI/UX", max: 100 },
            { name: "VueJs", max: 100 },
            { name: "ReactJs", max: 100 },
          ],
        },
        series: [
          {
            name: "Frontend Skills",
            type: "radar",
            data: [
              {
                value: [80, 80, 95, 75, 85, 60],
                name: "Frontend Skills",
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
