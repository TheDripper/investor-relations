<template>
  <div>
    <Nuxt />
  </div>
</template>

<style lang="scss">
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
.icons {
  img {
    max-width: 100px;
  }
}
@font-face {
  font-family: "heading";
  src: url("/head-book.ttf");
}
@font-face {
  font-family: "body-bold";
  src: url("/body-bold.ttf");
}
@font-face {
  font-family: "body-heavy";
  src: url("/body-heavy.ttf");
}
@font-face {
  font-family: "body-light";
  src: url("/body-light.ttf");
}
@font-face {
  font-family: "body-reg";
  src: url("/body-reg.ttf");
}
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "heading";
  color: #252525;
}
.button {
  font-family: "body-bold";
  font-size: 16px;
  color: #252525;
  text-transform: uppercase;
  text-decoration: none;
  @apply p-4 pr-12 border-2 rounded relative;
  border-color: #252525;
  display: inline-block;
  min-width: 315px;
  &:after {
    content: url("/TriangleDark.svg");
    @apply absolute;
    right: 20px;
    top: 50%;
    transform: translateY(-50%);
  }
}
.hero {
  background-image: url("/Benefits.jpg");
  background-size: cover;
  background-position: center;
  height: 600px;
  h1 {
    color: white;
  }
}
.bg-grey {
  background: linear-gradient(to right, #191919, #282828);
  p {
    color: white;
  }
  .button {
    color: #a6a6a6;
    border-color: #a6a6a6;
    min-width: none;
    &:after {
      content: url("/Triangle.svg");
    }
  }
}
h1 {
  font-size: 80px;
  line-height: 1;
}
h3 {
  color: #948477;
  font-size: 20px;
  font-family: "body-bold";
}
p {
  font-family: "body-reg";
}

.border-grey {
  border-color: #444444 !important;
}
.border-light-grey {
  border-color: #a6a6a6 !important;
}
h2 {
  font-size: 50px;
}
p,
li,
a {
  font-family: "body-reg";
  color: #494949;
}
a {
  text-decoration: underline;
}
.text-green {
  color: #376205 !important;
}
.font-bold {
  font-family: "body-heavy" !important;
}
</style>
