<script setup lang="ts">
import Nav from './components/Nav.vue'
</script>

<template>
<div>
  <header>
    <Nav/>
  </header>

  <div class="header">
    <h1 class="brandname" id="brandname">Wormwood</h1>
  </div>
  <main>
    <div class="icons">
      <div class="icon-item">
        <img src = "tree.svg" id="tree" alt="tree" class="icon"/>
        <h2>Tree</h2>
        <hr/>
        <p>Faithful decrepit chaos enlightenment dead transvaluation against endless. Ultimate zarathustra insofar law superiority society chaos. Overcome dead insofar truth law. Decrepit horror enlightenment love sea snare will evil morality sexuality sea salvation. Will self abstract.</p>
      </div>
      <div class="icon-item">
        <img src = "plant.svg" alt="plant" class="icon"/>
        <h2>Plant</h2>
        <hr/>
        <p>Endless merciful war inexpedient play chaos self hatred reason war prejudice. Pinnacle victorious faith overcome law law ideal superiority spirit spirit hope. Reason revaluation against gains selfish derive passion ocean evil horror. Madness ocean truth.</p>
      </div>
    </div>
    <hr/>
    <div>
      <h1 style="margin-left: 1.25rem;">About us</h1>
      <p style="margin-left: 1.625rem;">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Gravida quis blandit turpis cursus in hac habitasse platea. Sed vulputate odio ut enim blandit volutpat maecenas volutpat. Nunc id cursus metus aliquam. Nisl tincidunt eget nullam non. Velit scelerisque in dictum non. Ac turpis egestas sed tempus urna. Dignissim suspendisse in est ante in nibh. Odio facilisis mauris sit amet massa vitae. Libero nunc consequat interdum varius sit amet mattis vulputate enim. Tincidunt id aliquet risus feugiat in ante metus dictum.
<br/>
<br/>
Urna molestie at elementum eu facilisis sed odio. Dignissim diam quis enim lobortis scelerisque fermentum. Lorem ipsum dolor sit amet consectetur adipiscing. Eu scelerisque felis imperdiet proin fermentum leo vel orci porta. Hendrerit dolor magna eget est lorem ipsum dolor. Tortor dignissim convallis aenean et tortor at risus viverra. Cursus turpis massa tincidunt dui ut ornare lectus. Arcu cursus vitae congue mauris rhoncus. Morbi non arcu risus quis varius quam. Sed risus ultricies tristique nulla aliquet enim. Aliquet bibendum enim facilisis gravida.
<br/>
<br/>
Id aliquet risus feugiat in ante metus dictum at tempor. Sit amet est placerat in egestas. Tincidunt arcu non sodales neque sodales ut. Proin sed libero enim sed faucibus turpis. Sed adipiscing diam donec adipiscing. Venenatis urna cursus eget nunc scelerisque viverra mauris in. Scelerisque eu ultrices vitae auctor eu augue ut. Tortor consequat id porta nibh. Aliquet lectus proin nibh nisl condimentum. Tempor id eu nisl nunc mi ipsum faucibus vitae aliquet. In hac habitasse platea dictumst vestibulum rhoncus est. Nunc mattis enim ut tellus elementum sagittis. Ac auctor augue mauris augue neque gravida in fermentum. Nibh cras pulvinar mattis nunc sed. Vulputate dignissim suspendisse in est ante in nibh mauris cursus. Et malesuada fames ac turpis. Dui vivamus arcu felis bibendum ut tristique et egestas quis. Sociis natoque penatibus et magnis dis. Elementum pulvinar etiam non quam lacus. Sit amet massa vitae tortor condimentum lacinia quis vel.
      </p>
    </div>
  </main>
</div>
</template>

<style>
@import './assets/base.css';

div.header {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  padding: 0;
  background: linear-gradient( rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3) ), url('/forrest.png') no-repeat center center fixed;
  background-size: cover;
  background-attachment: inherit;
  margin-bottom: 0.75rem;
}

.header {
  font-size: 2em;
  font-weight: 900;
  line-height: 2em;
}

.brandname {
  /* used a vuejs gradient lookalike on accident lmfao */
  margin: 0;
  width: fit-content;
  height: auto;
  background: rgb(3,192,74);
  background: linear-gradient(90deg, rgba(3,192,74,1) 0%, rgba(0,251,255,1) 100%); 
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
}

main {
  min-height: 50vh;
}

.icons {
  display: grid;
  grid-template-columns: auto auto;
  grid-template-rows: auto;
  justify-content: space-evenly;
  justify-items: center;
  align-content: space-evenly;
  align-items: center;
}

.icon-item {
  text-align: center;
  width: 40%;
}

.icon {
  width: 64px;
  height: 64px;
}

#tree {
  filter: invert(69%) sepia(16%) saturate(1431%) hue-rotate(44deg) brightness(98%) contrast(95%);
}

h2 {
  margin: 0;
}

hr {
  margin: 2px;
}
</style>