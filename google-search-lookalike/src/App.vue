<template>
<div>
  <header>
    <div class="float-left">
      <span style="color: #FFF;">Gaagle</span>
      <input class="search" />
      <svg
        focusable="false"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        class="search-icon"
      >
        <path
          d="M15.5 14h-.79l-.28-.27A6.471 6.471 0 0 0 16 9.5 6.5 6.5 0 1 0 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"
        ></path>
      </svg>
      <div class="options">
        <div class="items">
          <div class="selected"></div>
          <div class="notselected" id="first"></div>
          <div class="notselected" id="second"></div>
          <div class="notselected" id="third"></div>
          <div class="notselected" id="forth"></div>
          <div class="notselected" id="fifth"></div>
        </div>
      </div>
    </div>
    <div class="float-right">
      <div class="apps-icon"></div>
      <div class="settings-icon"></div>
      <div class="user-icon"></div>
    </div>
  </header>
  <hr />

  <main>
    <div class="query-time"></div>
    <div class="results">
      <div class="result-item">
        <div class="result-description">
        </div>
      </div>
      <div class="result-item" id="two">
        <div class="result-description">
        </div>
      </div>
      <div class="result-item" id="three">
        <div class="result-description">
        </div>
      </div>
      <div class="result-item" id="four">
        <div class="result-description">
        </div>
      </div>
      <div class="result-item" id="five">
        <div class="result-description">
        </div>
      </div>
      <div class="result-item" id="six">
        <div class="result-description">
        </div>
      </div>
      <div class="result-item" id="seven">
        <div class="result-description">
        </div>
      </div>
      <div class="result-item" id="eight">
        <div class="result-description">
        </div>
      </div>
      <div class="result-item" id="nine">
        <div class="result-description">
        </div>
      </div>
      <div class="result-item" id="ten">
        <div class="result-description">
        </div>
      </div>
      <div class="fake-pagnate">Gaaaaaaaaaagle
        </div>
    </div>
  </main>
  </div>
</template>

<style>
@import "./assets/base.css";
</style>
