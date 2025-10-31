<template>


  <head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css">
    <!-- <meta charset="UTF-8"> -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  </head>
  <div class="main">
    <div class="section header">
      <div class="title">
        <img class="mat-icon" src="/icon.png" alt="DART icon">
        GUI Knowledge Bench
      </div>
      <div class="subtitle">
        Revealing the Knowledge Gap Behind VLM Failures in GUI Tasks
      </div>

      <div class="author-list">
       <span class="author">
          <el-link href="https://scholar.google.com/citations?user=DSN0fGIAAAAJ&hl=en">Chenrui Shi</el-link>
          <span class="ind">1,2</span>,
        </span>
        <span class="author">
          <el-link href="">Zedong Yu</el-link>
          <span class="ind">3,2</span>,
        </span>
        <span class="author">
          <el-link href="https://zhigao2017.github.io/">Zhi Gao</el-link>
          <span class="ind">1,2</span>,
        </span>
        <span class="author">
          <el-link href="">Ruining Feng</el-link>
          <span class="ind">4,2</span>,
        </span>
        <span class="author">
          <el-link href="">Enqi Liu</el-link>
          <span class="ind">2,4</span>,
        </span>
        <span class="author">
          <el-link href="https://wu-yuwei-bit.github.io/">Yuwei Wu</el-link>
          <span class="ind">1,5&#9993;</span>,
        </span>
        <span class="author">
          <el-link href="https://scholar.google.com/citations?user=Sl6TV7gAAAAJ&hl=en">Yunde Jia</el-link>
          <span class="ind">5</span>,
        </span>
        <span class="author">
          <el-link href="">Liuyu Xiang</el-link>
          <span class="ind">4</span>,
        </span>
        <span class="author">
          <el-link href="">Zhaofeng He</el-link>
          <span class="ind">4</span>,
        </span>
        <span class="author">
          <el-link href="https://liqing.io/">Qing Li</el-link>
          <span class="ind">2&#9993;</span>
        </span>
      </div>
      <div class="author-list">
        <span class="org">
          <span class="ind">1</span>
          BIT
        </span>
        <span class="org">
          <span class="ind">2</span>
          BIGAI
        </span>
        <span class="org">
          <span class="ind">3</span>
          BUPT 
        </span>
        <span class="org">
          <span class="ind">4</span>
          THU
        </span>
        <span class="org">
          <span class="ind">5</span>
          Shenzhen MSU-BIT University
        </span>
      </div>

      <span class="link-block">
        <a href="https://arxiv.org/abs/2510.26098" class="external-link button is-normal is-rounded is-dark">
          <span class="icon">
            <svg xmlns="http://www.w3.org/2000/svg" width="1.0em" height="1.0em" viewBox="0 0 24 24">
              <path fill="currentColor"
                d="M3.842 0a1 1 0 0 0-.922.608c-.153.369-.044.627.294 1.111l6.919 8.36l-1.023 1.106a1.04 1.04 0 0 0 .003 1.423l1.23 1.313l-5.44 6.444c-.28.3-.453.823-.297 1.199a1.025 1.025 0 0 0 .959.635a.91.91 0 0 0 .689-.34l5.783-6.126l7.49 8.005a.85.85 0 0 0 .684.26a.96.96 0 0 0 .877-.615c.158-.377-.017-.75-.306-1.14L13.73 13.9l1.064-1.13a.963.963 0 0 0 .009-1.316L4.633.464S4.26.01 3.867 0zm0 .272h.017c.218.005.487.272.564.364l.005.006l.005.005l10.17 10.99a.69.69 0 0 1-.008.946l-1.066 1.133l-1.498-1.772l-8.6-10.39c-.328-.472-.352-.619-.26-.841a.73.73 0 0 1 .671-.44Zm14.341 1.57a.88.88 0 0 0-.655.242l-5.696 6.158l1.694 1.832l5.309-6.514c.325-.433.479-.66.325-1.029a1.12 1.12 0 0 0-.977-.689m-7.655 12.282l1.318 1.414l-5.786 6.13a.65.65 0 0 1-.496.26a.75.75 0 0 1-.706-.467c-.112-.269.036-.687.244-.909l.005-.005l.005-.006z" />
            </svg>
          </span>
          <span>arXiv</span>
        </a>
      </span>
      <span class="link-block">
        <a href="https://github.com/Kendrick-Stein/GUI_Knowledge_Bench_Official_Repo?tab=readme-ov-file" class="external-link button is-normal is-rounded is-dark">
          <span class="icon">
            <i class="fab fa-github"></i>
          </span>
          <span>Code</span>
        </a>
      </span>

      <!-- Data Link. need changing -->
      <span class="link-block">
        <a target="_blank" href="https://huggingface.co/datasets/KendrickShi/GUI-Knowledge-Bench"
          class="external-link button is-normal is-rounded is-dark">
          <span class="icon">
            <i class="fa fa-database"></i>
          </span>
          <span>Dataset</span>
        </a>
      </span>

      
      <!-- <span class="link-block">
 
        <a target="_blank" href="https://li-qing-fire.hf.space"
          class="external-link button is-normal is-rounded is-dark">
          <span class="icon">
            <i class="fa fa-images"></i>
          </span>
          <span>Demo</span>
        </a>
      </span> -->
      <!-- <span class="link-block">
 
        <a target="_blank" href="https://x.com/Sealiqing/status/1819279627438973133"
          class="external-link button is-normal is-rounded is-dark">
          <span class="icon">
<svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="1.0em" height="1.0em" viewBox="0,0,256,256">
<g fill="#e9e9e9" fill-rule="nonzero" stroke="none" stroke-width="1" stroke-linecap="butt" stroke-linejoin="miter" stroke-miterlimit="10" stroke-dasharray="" stroke-dashoffset="0" font-family="none" font-weight="none" font-size="none" text-anchor="none" style="mix-blend-mode: normal"><g transform="scale(5.12,5.12)"><path d="M6.91992,6l14.2168,20.72656l-14.9082,17.27344h3.17773l13.13867,-15.22266l10.44141,15.22266h10.01367l-14.87695,-21.6875l14.08008,-16.3125h-3.17578l-12.31055,14.26172l-9.7832,-14.26172z"></path></g></g>
</svg>
          </span>
          <span>Twitter</span>
        </a>
      </span> -->
      <!-- <span class="link-block">
            <a href="file/clova_cvpr24_poster.pdf"
               class="external-link button is-normal is-rounded is-dark">
              <span class="icon">
                  <i class="fas fa-file-pdf"></i>
              </span>
              <span>Poster (CVPR'24)</span>
            </a>
          </span> -->

      <!-- <span class="link-block">
            <a href="file/clova_slides.pdf"
               class="external-link button is-normal is-rounded is-dark">
              <span class="icon">
                  <i class="fas fa-file-pdf"></i>
              </span>
              <span>Slides</span>
            </a>
          </span> -->

    </div>

    <div class="tldr">
      <p><b>TL;DR</b> The paper presents GUI Knowledge Bench to assess the knowledge gaps in vision-language models (VLMs) for GUI task automation, revealing limitations in understanding system states, predicting actions, and verifying task completion.</p>
    </div>

    <div class="section">
      <el-card class="teaser">
        <el-image src="./stats/1.png"></el-image>
      </el-card>
    </div>


    <div class="section">
      <div class="section-title">Introduction</div>
      <p class="intro">
        The paper introduces GUI Knowledge Bench, a new benchmark to evaluate the GUI knowledge of large vision-language models (VLMs) for GUI task automation. By analyzing failure patterns in GUI tasks, the authors identify three critical knowledge dimensions: interface perception, interaction prediction, and instruction understanding. The benchmark includes 3,483 multiple-choice and yes/no questions spanning six platforms (Web, Android, MacOS, Windows, Linux, iOS) and 292 applications. Key findings indicate that current VLMs struggle with perceiving system states, predicting action outcomes, and verifying task completion. The work provides insights for improving GUI agent training and highlights the need to enrich VLMs with domain-specific GUI knowledge.
      </p>
    </div>


    <div class="section">
      <div class="section-title">GUI Knowledge Bench </div>
      <el-scrollbar height="600px" always>
        <div class="teaser-list">
          <el-card class="teaser">
            <p class="intro">
            Example questions for Interface Perception:
            </p>
            <el-image src="./stats/2.png" fit="contain"></el-image>
          </el-card>
          <el-card class="teaser">
            <p class="intro">
            Example questions for Interaction Prediction:
            </p>
            <el-image src="./stats/4.png" fit="contain"></el-image>
          </el-card>
          <el-card class="teaser">
            <p class="intro">
            Example questions for Instruction Understanding:
            </p>
            <el-image src="./stats/3.png" fit="contain"></el-image>
          </el-card>
        </div>
      </el-scrollbar>
    </div>

    <div class="section">
      <div class="section-title">Statistics</div>
      <el-carousel class="stats-carousel" autoplay :interval="8000" arrow="always" indicator-position="outside" :pause-on-hover="false">
        <el-carousel-item>
          <el-card class="teaser">
            <el-image src="./stats/question_type_pie.png" fit="contain"></el-image>
          </el-card>
        </el-carousel-item>
        <el-carousel-item>
          <el-card class="teaser">
            <el-image src="./stats/images_per_question_bar.png" fit="contain"></el-image>
          </el-card>
        </el-carousel-item>
        <el-carousel-item>
          <el-card class="teaser">
            <el-image src="./stats/app_category_wordcloud.png" fit="contain"></el-image>
          </el-card>
        </el-carousel-item>
        <el-carousel-item>
          <el-card class="teaser">
            <el-image src="./stats/app_category_bar.png" fit="contain"></el-image>
          </el-card>
        </el-carousel-item>
        <el-carousel-item>
          <el-card class="teaser">
            <el-image src="./stats/image_sizes_top15_pie.png" fit="contain"></el-image>
          </el-card>
        </el-carousel-item>
      </el-carousel>
    </div>
    
    <div class="section">
      <div class="section-title">Experimental Results</div>
      <el-card class="leaderboard-card">
        <div class="table-caption">
          Performance on GUI Knowledge Bench across three dimensions.
        </div>
        <div class="table-wrap">
          <el-table
            :data="leaderboardData"
            border
            stripe
            size="small"
            style="width: 100%"
            :cell-class-name="cellClassName"
          >
            <el-table-column type="index" label="#" width="56" fixed="left" />
            <el-table-column prop="model" label="Model" fixed="left" min-width="180" />

            <el-table-column label="Interface Perception">
              <el-table-column prop="state" label="state" sortable min-width="110" :formatter="pctFormatter" />
              <el-table-column prop="widget" label="widget" sortable min-width="110" :formatter="pctFormatter" />
              <el-table-column prop="layout" label="layout" sortable min-width="110" :formatter="pctFormatter" />
            </el-table-column>

            <el-table-column label="Interaction Prediction">
              <el-table-column prop="effect" label="effect" sortable min-width="110" :formatter="pctFormatter" />
              <el-table-column prop="type" label="type" sortable min-width="110" :formatter="pctFormatter" />
              <el-table-column prop="parameter" label="parameter" sortable min-width="120" :formatter="pctFormatter" />
            </el-table-column>

            <el-table-column label="Instruction Understanding">
              <el-table-column prop="goal" label="goal" sortable min-width="110" :formatter="pctFormatter" />
              <el-table-column prop="plan" label="plan" sortable min-width="110" :formatter="pctFormatter" />
            </el-table-column>

            <el-table-column prop="overall" label="Overall" sortable min-width="120" :formatter="pctFormatter" />
          </el-table>
        </div>
      </el-card>
    </div>

    

  </div>
  

  <section class="section" id="BibTeX" style="text-align: left;">
    <div class="container is-max-desktop content" style="max-width: 100%; margin: 0 auto;">
      <div class="bibtex-header">
        <h3 class="title" style="font-size: small;">
          BibTeX
        </h3>
        <button @click="copyBibtex" class="copy-button" :class="{ 'copied': copySuccess }">
          <i class="fas" :class="copySuccess ? 'fa-check' : 'fa-copy'"></i>
          {{ copySuccess ? 'Copied!' : 'Copy' }}
        </button>
      </div>
      <div class="bibtex-container">
        <pre><code class="language-bibtex">

@article{Shi2025GUIBench,
  title = {GUI Knowledge Bench: Revealing the Knowledge Gap Behind VLM Failures in GUI Tasks},
  author={Chenrui Shi, Zedong YU, Zhi Gao, Ruining Feng, Enqi Liu, Yuwei Wu, Yunde Jia, Liuyu Xiang, Zhaofeng He, Qing Li},
  journal={arXiv preprint arXiv:XXXX.XXXXX},
  year={2025}
  url = {https://arxiv.org/abs/2510.26098}
}
</code></pre>
      </div>
    </div>
  </section>
  <div class="footer">
    This website is inspired by <el-link href="https://mathvista.github.io/">MathVista</el-link> and <el-link
      href="https://nerfies.github.io/">Nerfies</el-link>.
  </div>
</template>

<script setup>
// import Dialog from './Dialog.vue'

import { onMounted, onUnmounted, ref, computed } from 'vue'

const dataset1 = ref([])
const loadData1 = async () => {
  const resp1 = await fetch('./data/demo-100k.json')
  dataset1.value = await resp1.json()
}

const dataset2 = ref([])
const loadData2 = async () => {
  const resp2 = await fetch('./data/demo-1m.json')
  dataset2.value = await resp2.json()
}

const dataset3 = ref([])
const loadData3 = async () => {
  const resp3 = await fetch('./data/demo-bench.json')
  dataset3.value = await resp3.json()
}

// Leaderboard data and highlighting logic
const leaderboardRaw = [
  { model: 'GLM-4.5', state: 49.54, widget: 48.10, layout: 53.55, effect: 27.07, type: 17.55, parameter: 38.13, goal: 30.87, plan: 91.91 },
  { model: 'Claude-Sonnet-4', state: 70.18, widget: 78.44, layout: 78.06, effect: 41.55, type: 62.52, parameter: 45.75, goal: 63.78, plan: 94.82 },
  { model: 'Doubao-V-Pro', state: 72.48, widget: 83.65, layout: 81.29, effect: 68.10, type: 75.64, parameter: 52.17, goal: 33.07, plan: 94.17 },
  { model: 'Gemini-2.5-Pro', state: 81.19, widget: 84.36, layout: 87.10, effect: 71.72, type: 73.25, parameter: 60.31, goal: 66.46, plan: 92.56 },
  { model: 'GPT-5-Chat', state: 78.90, widget: 84.12, layout: 88.39, effect: 73.10, type: 71.55, parameter: 57.89, goal: 67.40, plan: 91.26 },
  { model: 'O3', state: 83.03, widget: 84.12, layout: 88.39, effect: 76.55, type: 75.98, parameter: 60.31, goal: 67.56, plan: 95.47 },
  { model: 'Qwen2.5VL-7B', state: 53.21, widget: 67.77, layout: 60.00, effect: 52.59, type: 50.60, parameter: 44.54, goal: 17.01, plan: 48.87 },
  { model: 'Qwen2.5VL-72B', state: 69.72, widget: 77.49, layout: 80.00, effect: 62.93, type: 64.91, parameter: 44.89, goal: 61.89, plan: 85.44 },
  { model: 'UITARS-1.5-7B', state: 49.54, widget: 59.48, layout: 59.35, effect: 22.76, type: 59.11, parameter: 43.50, goal: 39.84, plan: 55.34 },
]

const toFixed2 = (n) => Number(n.toFixed(2))
const overallOf = (r) => toFixed2((r.state + r.widget + r.layout + r.effect + r.type + r.parameter + r.goal + r.plan) / 8)

const leaderboardData = ref(
  leaderboardRaw
    .map(r => ({ ...r, overall: overallOf(r) }))
    .sort((a, b) => b.overall - a.overall)
)

const metricCols = ['state', 'widget', 'layout', 'effect', 'type', 'parameter', 'goal', 'plan']

const columnMax = computed(() => {
  const m = {}
  for (const c of metricCols) {
    m[c] = Math.max(...leaderboardData.value.map(r => r[c] ?? -Infinity))
  }
  return m
})

// Highlight best cell per column
const cellClassName = ({ row, column }) => {
  const prop = column.property
  if (metricCols.includes(prop)) {
    const isBest = Math.abs(row[prop] - columnMax.value[prop]) < 1e-6
    return isBest ? 'best-cell' : ''
  }
  return ''
}

// Percentage formatter
const pctFormatter = (_row, _column, cellValue) => `${toFixed2(cellValue)}%`
// Copy functionality for BibTeX
const copySuccess = ref(false)

// Carousel logic
const carouselRef = ref(null)
const activeIndex = ref(0)
const direction = ref(1) // 1 forward, -1 backward
let timer = null

const onCarouselChange = (newIndex) => {
  activeIndex.value = newIndex
}

const bibtexText = `@article{li2025dart,
  title = {GUI Knowledge Bench: Revealing the Knowledge Gap Behind VLM Failures in GUI Tasks},
  author={Chenrui Shi, Zedong YU, Zhi Gao, Ruining Feng, Enqi Liu, Yuwei Wu, Yunde Jia, Liuyu Xiang, Zhaofeng He, Qing Li},
  journal={arXiv preprint arXiv:XXXX.XXXXX},
  year={2025}
  url = {https://arxiv.org/abs/xxxxx}
}`

const copyBibtex = async () => {
  try {
    await navigator.clipboard.writeText(bibtexText)
    copySuccess.value = true
    setTimeout(() => {
      copySuccess.value = false
    }, 2000)
  } catch (err) {
    console.error('Failed to copy: ', err)
    // Fallback for older browsers
    const textArea = document.createElement('textarea')
    textArea.value = bibtexText
    document.body.appendChild(textArea)
    textArea.select()
    document.execCommand('copy')
    document.body.removeChild(textArea)
    copySuccess.value = true
    setTimeout(() => {
      copySuccess.value = false
    }, 2000)
  }
}

onMounted(() => {
  timer = setInterval(() => {
    if (activeIndex.value === 0) direction.value = 1
    if (activeIndex.value === 2) direction.value = -1

    if (direction.value === 1) {
      carouselRef.value?.next()
    } else {
      carouselRef.value?.prev()
    }
  }, 4000)

  loadData1()
  loadData2()
  loadData3()
})

onUnmounted(() => {
  if (timer) clearInterval(timer)
})
</script>






<style scoped>
.main {
  text-align: center;
  color: #23272f;
  font-family: 'Inter', 'Helvetica Neue', Arial, sans-serif;
  max-width: 1300px;
  margin: 0 auto;
  padding: 0 24px;
  background: linear-gradient(120deg, #f8fbff 0%, #f3f6fa 100%);
}

.header {
  margin: 56px 0 32px 0 !important;
}

.title {
  font-size: 3.8em;
  font-weight: 800;
  color: #34618D;
  letter-spacing: -1px;
  margin-bottom: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 16px;
}

.subtitle {
  font-size: 2.1em;
  color: #3572afff;
  font-weight: 500;
  line-height: 1.3;
  max-width: 1100px;
  margin: 0 auto 12px auto;
  letter-spacing: 0.01em;
}

.author-list {
  margin: 18px 0 0 0;
  line-height: 1.7;
  font-size: 1.08em;
  color: #2b3a4b;
}

.author a {
  font-size: 1em;
  font-weight: 600;
  color: #34618D;
  text-decoration: none;
  border-bottom: 1px dotted #34618D;
  transition: color 0.2s, border-bottom 0.2s;
}
.author a:hover {
  color: #34618D;
  border-bottom: 1px solid #34618D;
}

.org {
  margin: 0 4px;
  color: #607d8b;
  font-size: 0.98em;
}

.ind {
  font-size: 0.7em;
  vertical-align: super;
  color: #90a4ae;
}

.section {
  margin: 36px 0;
  padding: 0 10px;
}

.tldr {
  text-align: left;
  font-size: 1.08em;
  max-width: 1100px;
  line-height: 1.6;
  margin: 28px auto 24px auto;
  padding: 18px 24px;
  background: linear-gradient(90deg, #91b5d9ff 0%, #f5fafd 100%);
  border-left: 4px solid #34618D;
  border-radius: 8px;
  box-shadow: 0 2px 8px 0 rgba(123, 31, 162, 0.04);
}

.section-title {
  margin: 32px 0 18px;
  font-size: 1.7em;
  font-weight: 700;
  color: #34618D;
  text-align: left;
  letter-spacing: 0.01em;
}

.conference {
  text-align: center;
  margin: 15px;
  font-size: 1.2em;
  color: #666;
}

.uns {
  text-decoration: underline;
  text-decoration-color: #34618D;
}

.mat-icon {
  width: 1.3em;
  height: 1.3em;
  margin-right: 0.1em;
  vertical-align: middle;
  display: inline-block;
}

.teaser, .poster, .stats-img-1 {
  max-width: 98%;
  margin: 24px auto;
  border-radius: 12px;
  background: #fff;
  box-shadow: 0 2px 12px 0 rgba(123, 31, 162, 0.06);
  border: 1px solid #34618D;
  overflow: hidden;
}

.stats-img {
  height: auto;
  max-width: 100%;
  margin: 15px auto;
}

.teaser-list {
  padding-right: 8px;
}

.intro {
  text-align: justify;
  font-size: 1.08em;
  max-width: 1100px;
  line-height: 1.6;
  margin: 0 auto 12px auto;
  color: #23272f;
}

.link-block {
  margin: 18px 0;
}

.external-link {
  display: inline-flex;
  align-items: center;
  padding: 10px 22px;
  margin: 6px;
  border: none;
  border-radius: 6px;
  background: linear-gradient(90deg, #34618D 0%, #34618D 100%);
  color: #fff;
  text-decoration: none;
  font-size: 1em;
  font-weight: 600;
  box-shadow: 0 2px 8px 0 rgba(123, 31, 162, 0.08);
  transition: background 0.2s, box-shadow 0.2s, transform 0.1s;
}
.external-link:hover {
  background: linear-gradient(90deg, #34618D 0%, #34618D 100%);
  box-shadow: 0 4px 16px 0 rgba(123, 31, 162, 0.13);
  transform: translateY(-2px) scale(1.03);
}
.external-link .icon {
  margin-right: 10px;
  color: #f3e5f5;
}

.bibtex-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 8px;
}

.copy-button {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 6px 12px;
  background: #34618D;
  border: 1px solid #34618D;
  border-radius: 6px;
  color: #fdfdfdff;
  font-size: 0.9em;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.2s ease;
}

.copy-button:hover {
  background: #34618D;
  color: #fff;
  border-color: #34618D;
  transform: translateY(-1px);
  box-shadow: 0 2px 8px 0 rgba(123, 31, 162, 0.15);
}

.copy-button.copied {
  background: #4caf50;
  color: #fff;
  border-color: #388e3c;
}

.copy-button i {
  font-size: 0.85em;
}

.bibtex-container {
  background: #f5fafd;
  padding: 1.2em;
  border-radius: 8px;
  text-align: left;
  white-space: pre;
  overflow-x: auto;
  border: 1px solid #34618D;
  margin: 18px 0;
}

pre {
  margin: 0;
  font-family: 'Fira Mono', 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, monospace;
}

code {
  font-family: 'Fira Mono', 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, monospace;
  color: #23272f;
  font-size: 0.98em;
}

.footer {
  color: #90a4ae;
  margin: 60px 0 30px;
  font-size: 0.98em;
  text-align: center;
}
.footer a {
  color: #34618D;
  text-decoration: none;
  border-bottom: 1px dotted #34618D;
  transition: color 0.2s, border-bottom 0.2s;
}
.footer a:hover {
  color: #34618D;
  border-bottom: 1px solid #34618D;
}

@media (max-width: 900px) {
  .main {
    max-width: 100vw;
    padding: 0 6px;
  }
  .title {
    font-size: 2.2em;
  }
  .subtitle {
    font-size: 1.1em;
  }
  .section {
    padding: 0 2px;
  }
  .stats-img-1, .teaser, .poster {
    max-width: 100%;
  }
  .tldr, .intro {
    max-width: 98vw;
  }
}

.research-bar {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 18px;
  padding: 18px 0 8px 0;
  background: transparent;
  font-size: 1.08em;
  flex-wrap: wrap;
  position: relative;
}
.research-title {
  color: #34618D;
  font-weight: 700;
  margin-right: 8px;
}
.research-link {
  display: inline-flex;
  align-items: center;
  padding: 6px 16px;
  border-radius: 6px;
  background: #34618D;
  color: #34618D;
  text-decoration: none;
  font-weight: 600;
  margin: 0 2px;
  transition: background 0.18s, color 0.18s, box-shadow 0.18s;
  box-shadow: 0 1px 4px 0 rgba(123, 31, 162, 0.06);
}
.research-link:hover {
  background: #34618D;
  color: #fff;
  box-shadow: 0 2px 8px 0 rgba(123, 31, 162, 0.13);
}
.conf-tag {
  font-size: 0.95em;
  font-weight: 400;
  color: #34618D;
  background: #34618D;
  border-radius: 4px;
  padding: 2px 6px;
  margin-left: 6px;
  transition: color 0.18s, background 0.18s;
}
.research-link:hover .conf-tag {
  color: #fff;
  background: #34618D;
}
.research-link-wrapper {
  position: relative;
  display: inline-block;
}
.preview-popup {
  display: none;
  position: absolute;
  left: 50%;
  top: 110%;
  transform: translateX(-50%);
  width: 1000px;
  height: 600px;
  background: rgba(255,255,255,0.95);
  border-radius: 10px;
  box-shadow: 0 8px 32px 0 rgba(123, 31, 162, 0.18);
  z-index: 100;
  opacity: 0;
  pointer-events: none;
  transition: opacity 0.25s;
  overflow: hidden;
}
.research-link-wrapper:hover .preview-popup {
  display: block;
  opacity: 1;
  pointer-events: auto;
}
.preview-popup iframe {
  width: 100%;
  height: 100%;
  border: none;
  opacity: 0.85;
  border-radius: 10px;
}
@media (max-width: 900px) {
  .preview-popup {
    display: none !important;
  }
}

.image-stack {
  display: flex;
  flex-direction: column; /* 上下排列 */
  gap: 0; /* 移除间距 */
}

.image-stack >>> .el-image {
  margin: 0; /* 避免 el-image 默认 margin */
  width: 100%;
}
.image-stack >>> .el-image__inner {
  width: 100%;
  height: 100%;
  object-fit: contain;
}
:deep(.el-carousel__container) {
  height: auto !important;
}
:deep(.el-carousel__item) {
  height: auto !important;
}

.dashed-separator {
  border-top: 2px dashed #888; /* 粗细和颜色 */
  margin: 12px 0; /* 上下间距 */
  width: 100%;

  /* 控制虚线段长，使用 border-image */
  border-top-style: dashed;
  border-top-width: 2px;
  border-image: repeating-linear-gradient(to right, #888 0, #888 8px, transparent 8px, transparent 16px) 1;
}
.stats-carousel {
  width: 900px;
  max-width: 100%;
  margin: 0 auto;
}
.stats-carousel :deep(.el-carousel__container) {
  width: 100%;
  aspect-ratio: 4 / 3;
  height: auto !important;
}
@media (max-width: 900px) {
  .stats-carousel {
    width: 100%;
  }
}
.stats-carousel :deep(.el-carousel__item) {
  height: 100% !important;
  display: flex;
  align-items: center;
  justify-content: center;
}
.stats-carousel :deep(.el-image) {
  width: 100%;
  height: 100%;
  display: block;
}
.stats-carousel :deep(.el-image__inner) {
  width: 100%;
  height: 100%;
  object-fit: contain;
  object-position: center center;
  display: block;
}
.stats-carousel :deep(.el-card__body) {
  height: 100%;
  padding: 0;
  display: flex;
  align-items: center;
  justify-content: center;
}
.stats-carousel .teaser {
  height: 100%;
  margin: 0;
  display: flex;
  border-radius: 12px;
}
.leaderboard-card {
  padding: 12px;
}
.table-caption {
  text-align: left;
  color: #607d8b;
  font-size: 0.95em;
  margin-bottom: 8px;
}
.table-wrap {
  width: 100%;
  overflow-x: auto;
  overflow-y: visible;
  border-radius: 8px;
  background: #fff;
  box-shadow: 0 2px 12px 0 rgba(123, 31, 162, 0.06);
  border: 1px solid #34618D;
}
.best-cell {
  font-weight: 700;
  color: #d35400;
  background: rgba(211, 84, 0, 0.10);
}
/* Sticky table header within el-table */
:deep(.el-table__header-wrapper) {
  position: sticky;
  top: 0;
  z-index: 5;
  background: #fff;
}
:deep(.el-table__header) {
  background: #fff;
}
</style>
