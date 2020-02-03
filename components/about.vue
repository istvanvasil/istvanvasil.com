<template>
  <div class="about">
    <div class="grid">
      <div class="profile">
        <p>
          My practice revolves around design as a holistic system, unconditional
          of the medium, including both digital and physical. I combine
          aesthetic principles with high functionality to create new ways of
          interaction and communication.
        </p>
        <p class="break-single">
          I currently work as a designer at
          <a href="https://sdl.se" target="_blank">Stockholm Design Lab.</a>
          Portfolio is availabe upon request.
        </p>
        <p class="break-single">
          Client experience includes Ericsson, The Nobel Prize, OneLab,
          Universal, S7 Airlines, NIO Formula E Team, Adidas, amongst others.
        </p>
        <p class="break-single">
          Contact
        </p>
        <p>
          <a href="mailto:info@istvanvasil.com">
            info@istvanvasil.com
          </a>
        </p>
        <p class="break-single">
          Also on
        </p>
        <p>
          <a href="https://twitter.com/istvanvasil" target="_blank">Twitter</a>,
          <a href="https://www.instagram.com/stvnvsl" target="_blank"
            >Instagram</a
          >,
          <a href="https://www.are.na/istvan-vasil" target="_blank">Arena</a>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'About'
}
</script>

<style>
.about {
  line-height: 1.125rem;
  padding: 0 1.5rem 0 1.5rem;
  margin-top: 4rem;
  margin-bottom: 6rem;
}

@media screen and (max-width: 600px) {
  .about {
    padding: 0 1rem 0 1rem;
    margin-top: 4rem;
    margin-bottom: 4rem;
  }
}

.profile {
  grid-column: 7/-1;
  max-width: 350px;
}

@media screen and (max-width: 600px) {
  .profile {
    grid-column: 5/-1;
  }
}
</style>
