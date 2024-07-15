<template>
    <div class="steps-indicator-component">
      <div class="progress-container">
        <div class="step-wrapper">
          <div class="step active">1</div>
          <div class="label">{{ startingPointLabel }}</div>
        </div>
        <div class="bars">
          <div class="bar-background"></div>
          <div class="progress" :style="{ width: `${percentage}%` }"></div>
        </div>
        <div class="step-wrapper">
          <div class="step" :class="{ active: percentage === 100 }">2</div>
          <div class="label" :style="{ opacity: percentage === 100 ? '1' : '0.5' }">Done!</div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      percentage: {
        type: Number,
        required: true
      },
      startingPointLabel: {
        type: String,
        required: true
      }
    }
  }
  </script>
  