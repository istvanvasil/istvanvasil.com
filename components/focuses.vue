<template>
  <div class="focuses-container">
    <div class="focuses responsive-type">
      <div class="grid">
        <div id="focus-one">
          <p>
            <span class="char1">D</span><span class="char2">e</span
            ><span class="char3">s</span><span class="char4">i</span
            ><span class="char5">g</span><span class="char6">n</span>
          </p>
          <p>
            <span class="char7">s</span><span class="char8">y</span
            ><span class="char9">s</span><span class="char10">t</span
            ><span class="char11">e</span><span class="char12">m</span
            ><span class="char13">s</span>
          </p>
        </div>
      </div>
      <div class="grid">
        <div id="focus-two">
          <p>
            <span class="char1">U</span><span class="char2">s</span
            ><span class="char3">e</span><span class="char4">r</span>
          </p>
          <p>
            <span class="char5">i</span><span class="char6">n</span
            ><span class="char7">t</span><span class="char8">e</span
            ><span class="char9">r</span><span class="char10">a</span
            ><span class="char11">c</span><span class="char12">t</span
            ><span class="char13">i</span><span class="char14">o</span
            ><span class="char15">n</span>
          </p>
        </div>
      </div>
      <div class="grid">
        <div id="focus-three">
          <p>
            <span class="char1">V</span><span class="char2">i</span
            ><span class="char3">s</span><span class="char4">u</span
            ><span class="char5">a</span><span class="char6">l</span>
          </p>
          <p>
            <span class="char8">c</span><span class="char9">o</span
            ><span class="char10">m</span><span class="char11">m</span
            ><span class="char12">u</span><span class="char13">n</span
            ><span class="char14">i</span><span class="char15">c</span
            ><span class="char16">a</span><span class="char17">t</span
            ><span class="char18">i</span><span class="char19">o</span
            ><span class="char20">n</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Focuses'
}
</script>

<style>
.focuses {
  margin-top: 6rem;
  padding: 0 1.5rem 0 1.5rem;
}

@media screen and (max-width: 600px) {
  .focuses {
    margin-top: 3rem;
    padding: 0 1rem 0 1rem;
  }
}

#focus-one {
  grid-column: 1/-1;
  margin-left: -0.85vw;
  margin-bottom: 2rem;
}

#focus-one .char2 {
  margin-left: -0.005em;
}

#focus-one .char5 {
  margin-left: -0.01em;
}

#focus-one .char6 {
  margin-left: -0.01em;
}

#focus-one .char9 {
  margin-left: -0.015em;
}

#focus-one .char12 {
  margin-left: -0.005em;
}

#focus-one .char13 {
  margin-left: -0.005em;
}

@media screen and (max-width: 600px) {
  #focus-one {
    margin-bottom: 2rem;
  }
}

#focus-two {
  grid-column: 7/-1;
  margin-left: -0.7vw;
  margin-bottom: 2rem;
}

#focus-two .char2 {
  margin-left: -0.015em;
}

#focus-two .char11 {
  margin-left: -0.015em;
}

#focus-two .char14 {
  margin-left: -0.005em;
}

#focus-two .char15 {
  margin-left: -0.008em;
}

@media screen and (max-width: 600px) {
  #focus-two {
    grid-column: 5/-1;
    margin-bottom: 2rem;
  }
}

#focus-three {
  grid-column: 2/-1;
}

#focus-three .char2 {
  margin-left: -0.005em;
}

#focus-three .char4 {
  margin-left: -0.003em;
}

#focus-three .char5 {
  margin-left: -0.008em;
}

#focus-three .char10 {
  margin-left: -0.01em;
}

#focus-three .char11 {
  margin-left: -0.01em;
}

#focus-three .char12 {
  margin-left: -0.01em;
}

#focus-three .char13 {
  margin-left: -0.01em;
}

#focus-three .char17 {
  margin-left: -0.01em;
}

#focus-three .char20 {
  margin-left: -0.005em;
}
</style>
