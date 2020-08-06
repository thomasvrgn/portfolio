<template>
  <div class="nessmc:hero">
    <div class="nessmc:hero-text">
      <div class="nessmc:container">
        <div class="nessmc:text-container">
          <h1 class="nessmc:title">
            Ness
          </h1>
          <span class="nessmc:job">
            Web developer
          </span>
          <p class="nessmc:description">
            Hey, I'm Ness, web developer for five years now. I'm specialized in integrating web mock-ups and learning web design. 
          </p>
          <div class="nessmc:buttons">
            <a href="" class="nessmc:button">
              <svg width="32" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M8 3C9.10457 3 10 3.89543 10 5V8H16C17.1046 8 18 8.89543 18 10C18 11.1046 17.1046 12 16 12H10V14C10 15.6569 11.3431 17 13 17H16C17.1046 17 18 17.8954 18 19C18 20.1046 17.1046 21 16 21H13C9.13401 21 6 17.866 6 14V5C6 3.89543 6.89543 3 8 3Z" fill="currentColor" /></svg>
            </a>
            <a href="" class="nessmc:button">
              <svg width="32" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 7C9.23858 7 7 9.23858 7 12C7 14.7614 9.23858 17 12 17C14.7614 17 17 14.7614 17 12C17 9.23858 14.7614 7 12 7ZM9 12C9 13.6569 10.3431 15 12 15C13.6569 15 15 13.6569 15 12C15 10.3431 13.6569 9 12 9C10.3431 9 9 10.3431 9 12Z" fill="currentColor" /><path d="M18 5C17.4477 5 17 5.44772 17 6C17 6.55228 17.4477 7 18 7C18.5523 7 19 6.55228 19 6C19 5.44772 18.5523 5 18 5Z" fill="currentColor" /><path fill-rule="evenodd" clip-rule="evenodd" d="M5 1C2.79086 1 1 2.79086 1 5V19C1 21.2091 2.79086 23 5 23H19C21.2091 23 23 21.2091 23 19V5C23 2.79086 21.2091 1 19 1H5ZM19 3H5C3.89543 3 3 3.89543 3 5V19C3 20.1046 3.89543 21 5 21H19C20.1046 21 21 20.1046 21 19V5C21 3.89543 20.1046 3 19 3Z" fill="currentColor" /></svg>
            </a>
            <a href="" class="nessmc:button">
              <svg width="32" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M9 3C7.89543 3 7 3.89543 7 5C7 5.74028 7.4022 6.38663 8 6.73244V17.2676C7.4022 17.6134 7 18.2597 7 19C7 20.1046 7.89543 21 9 21C9.74028 21 10.3866 20.5978 10.7324 20H11.9585C14.1676 20 15.9585 18.2091 15.9585 16V14.7324C16.5563 14.3866 16.9585 13.7403 16.9585 13C16.9585 11.8954 16.0631 11 14.9585 11C13.8539 11 12.9585 11.8954 12.9585 13C12.9585 13.7403 13.3607 14.3866 13.9585 14.7324V16C13.9585 17.1046 13.0631 18 11.9585 18H10.7324C10.5568 17.6964 10.3036 17.4432 10 17.2676V6.73244C10.5978 6.38663 11 5.74028 11 5C11 3.89543 10.1046 3 9 3Z" fill="currentColor" /></svg>
            </a>
          </div>
        </div>
      </div>
    </div>
    <div class="nessmc:hero-banner">
      <span></span>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  
})
</script>

<style lang="scss">
.nessmc\:hero {
  position: absolute;
  top: 50%;
  left: calc(100% - 792.5px);
  transform: translate(-50%, -50%);
  height: 50%;
  min-height: unset !important;
  width: 950px;
  border-radius: 25px;
  display: flex;
  @media (max-width: 1440px) {
    width: 75%;
    height: 75%;
    left: 50%;
  }
  @media (max-width: 1280px) {
    flex-flow: row wrap;
    height: 65%;
    width: 65%;
  }
  .nessmc\:hero-text {
    min-height: unset !important;
    display: flex;
    flex: 1 0 65%;
    background: white;
    border-radius: 25px 0 0 25px;
    @media (max-width: 1280px) {
      border-radius: 25px;
      text-align: center;
    } 
    .nessmc\:container {
      min-height: unset !important;
      display: flex;
      justify-content: center;
      align-items: center;
      .nessmc\:text-container {
        width: 50%;
        min-height: unset !important;
        margin: 0 auto;
        display: block;
        .nessmc\:title {
          font-family: 'Roboto Slab';
          font-weight: 400;
          font-size: 3rem;
          color: #243678;
        }
        .nessmc\:description {
          color: #999999;
        }
        .nessmc\:job {
          display: block;
          margin-bottom: 1.5rem;
          font-weight: 300;
          opacity: 0.7;
          color: #1c55d8;
          font-family: 'Roboto Slab';
        }
        .nessmc\:buttons {
          margin: 2rem 0 0;
          min-height: unset !important;
          .nessmc\:button {
            margin: 0 1rem;
            color: #cccccc;
            &:first-child {
              margin: 0 1rem 0 0;
            }
            &:last-child {
              margin: 0 0 0 1rem;
            }
            @media (max-width: 1280px) {
              margin: 0 1rem;
            }
          }
        }
      }
    }
    @media (max-width: 1440px) {
      flex: 1 0 50%;
    }
    @media (max-width: 1280px) {
      flex: 1 0 100%;
    }
  }
  .nessmc\:hero-banner {
    min-height: unset !important;
    display: flex;
    flex: 1 0 35%;
    background-image: url('../assets/logo.jpg');
    margin-left: -1px;
    background-position: center center;
    background-size: cover;
    filter: grayscale(100%);
    border-radius: 0 25px 25px 0;
    @media (max-width: 1440px) {
      flex: 1 0 50%;
    }
    @media (max-width: 1280px) {
      flex: 1 0 100%;
      display: none;
    }
  }
}
</style>