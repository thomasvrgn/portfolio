<template>
  <div class="nessmc:container">
    <nav class="nessmc:navbar">
      <div class="nessmc:navbar-item nessmc:navbar-start">
        <span class="nessmc:title">
          N
        </span>
      </div>
      <div class="nessmc:navbar-item nessmc:navbar-end">
        <span class="nessmc:button" @click=open>
          <svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M22 18.0048C22 18.5544 21.5544 19 21.0048 19H12.9952C12.4456 19 12 18.5544 12 18.0048C12 17.4552 12.4456 17.0096 12.9952 17.0096H21.0048C21.5544 17.0096 22 17.4552 22 18.0048Z" fill="currentColor" /><path d="M22 12.0002C22 12.5499 21.5544 12.9954 21.0048 12.9954H2.99519C2.44556 12.9954 2 12.5499 2 12.0002C2 11.4506 2.44556 11.0051 2.99519 11.0051H21.0048C21.5544 11.0051 22 11.4506 22 12.0002Z" fill="currentColor" /><path d="M21.0048 6.99039C21.5544 6.99039 22 6.54482 22 5.99519C22 5.44556 21.5544 5 21.0048 5H8.99519C8.44556 5 8 5.44556 8 5.99519C8 6.54482 8.44556 6.99039 8.99519 6.99039H21.0048Z" fill="currentColor" /></svg>
        </span>
      </div>
    </nav>
    <div class="nessmc:navbar-content" :class="{'nessmc:navbar-opened': this.opened}">
      <span></span>
      <span class="nessmc:close-button" @click=open>
        <svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M6.2253 4.81108C5.83477 4.42056 5.20161 4.42056 4.81108 4.81108C4.42056 5.20161 4.42056 5.83477 4.81108 6.2253L10.5858 12L4.81114 17.7747C4.42062 18.1652 4.42062 18.7984 4.81114 19.1889C5.20167 19.5794 5.83483 19.5794 6.22535 19.1889L12 13.4142L17.7747 19.1889C18.1652 19.5794 18.7984 19.5794 19.1889 19.1889C19.5794 18.7984 19.5794 18.1652 19.1889 17.7747L13.4142 12L19.189 6.2253C19.5795 5.83477 19.5795 5.20161 19.189 4.81108C18.7985 4.42056 18.1653 4.42056 17.7748 4.81108L12 10.5858L6.2253 4.81108Z" fill="currentColor" /></svg>
      </span>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data: () => ({
    opened: false
  }),
  methods: {
    open: function () : void {
      this.opened = !this.opened
    }
  }
})
</script>

<style lang="scss">
.nessmc\:container {
  position: absolute;
  .nessmc\:navbar {
    z-index: 1;
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
          background-color: #1c55d8;
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
          @media (max-width: 1280px) {
            color: #1c55d8;
          }
        }
      }
    }
  }
  .nessmc\:navbar-content {
    z-index: 2;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #1c55d8;
    left: -100%;
    transition: left 1s ease;
    &.nessmc\:navbar-opened {
      left: 0;
    }
    .nessmc\:close-button {
      display: inline-block;
      margin: 2rem;
      color: white;
      cursor: pointer;
    }
  }
}
</style>
