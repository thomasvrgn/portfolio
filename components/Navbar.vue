<template>
  <nav class="nessmc:navbar">
    <div class="nessmc:navbar-item nessmc:navbar-start">
      <span class="nessmc:title">
        N
      </span>
    </div>
    <div class="nessmc:navbar-item nessmc:navbar-end">
      <span class="nessmc:button">
        <svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M22 18.0048C22 18.5544 21.5544 19 21.0048 19H12.9952C12.4456 19 12 18.5544 12 18.0048C12 17.4552 12.4456 17.0096 12.9952 17.0096H21.0048C21.5544 17.0096 22 17.4552 22 18.0048Z" fill="currentColor" /><path d="M22 12.0002C22 12.5499 21.5544 12.9954 21.0048 12.9954H2.99519C2.44556 12.9954 2 12.5499 2 12.0002C2 11.4506 2.44556 11.0051 2.99519 11.0051H21.0048C21.5544 11.0051 22 11.4506 22 12.0002Z" fill="currentColor" /><path d="M21.0048 6.99039C21.5544 6.99039 22 6.54482 22 5.99519C22 5.44556 21.5544 5 21.0048 5H8.99519C8.44556 5 8 5.44556 8 5.99519C8 6.54482 8.44556 6.99039 8.99519 6.99039H21.0048Z" fill="currentColor" /></svg>
      </span>
    </div>
  </nav>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  
})
</script>

<style lang="scss">
.nessmc\:navbar {
  display: flex;
  flex-flow: row wrap;
  width: 100%;
  margin: 0 auto;
  position: absolute;
  padding: 2rem 2.5rem;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  .nessmc\:navbar-item {
    display: flex;
    min-height: unset !important;
    align-items: center;
    &.nessmc\:navbar-start {
      flex: 0 1 auto;
      padding: 0 0.5rem;
      .nessmc\:title {
        font-size: 2rem;
        background-color: #a71cd8;
        border-radius: 5px;
        padding: 0.5rem 1rem;
        color: white;
        font-weight: 800;
      }
    }
    &.nessmc\:navbar-end {
      flex: 1 1 auto;
      justify-content: flex-end;
      .nessmc\:button {
        color: white;
        cursor: pointer;
      }
    }
  }
}
</style>