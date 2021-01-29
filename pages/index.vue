<template>
  <div id="investor-relations">
    <div class="w-full hero pt-8">
      <div class="w-full mt-8 mb-32 flex items-center bg-grey py-16 px-8">
        <div class="flex flex-col pr-12">
          <h3>INVESTORS</h3>
          <h1>Investor Relations</h1>
        </div>
        <div class="flex flex-col pl-12 border-l border-grey">
          <p class="mb-8">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Donec ac
            odio tempor orci dapibus ultrices. Eu ultrices vitae auctor eu augue
            ut. Tellus elementum sagittis vitae et leo duis ut.
          </p>
          <div class="flex">
            <a href="#" class="button mr-4">2019 Annual Report</a>
            <a href="#" class="button">Investor Presentation</a>
          </div>
        </div>
      </div>
    </div>
    <div class="flex w-full mt-12 px-4 pb-12">
      <div style="flex:75%;">
        <h1>Press Releases</h1>
        <ul>
          <li>Link 1</li>
          <li>Link 1</li>
          <li>Link 1</li>
          <li>Link 1</li>
        </ul>
        <a href="#" class="button">View All Press Releases</a>
        <h1 class="mt-12">Earnings Releases</h1>
        <ul>
          <li>Link 1</li>
          <li>Link 1</li>
          <li>Link 1</li>
          <li>Link 1</li>
        </ul>
        <a href="#" class="button">View All Earnings Releases</a>
      </div>
      <div style="flex:25%;">
        <h3 class="text-green">HEADQUARTERS</h3>
        <p>Carriage Services, Inc.</p>
        <p>3040 Post Oak Boulevard Suite 300</p>
        <p>Houston, Texas 77056</p>
        <p>713.332.8400</p>
        <p>www.carriageservices.com</p>
      </div>
    </div>
    <h2>Stock Performance</h2>
    <img src="/stock.png" />
    <div class="flex w-full">
      <div class="flex w-full w-1/4 items-center justify-center icons">
        <img src="/print.svg" />
      </div>
      <div class="flex w-full w-1/4 items-center justify-center icons">
        <img src="/email.svg" />
      </div>
      <div class="flex w-full w-1/4 items-center justify-center icons">
        <img src="/rss.svg" />
      </div>
      <div class="flex w-full w-1/4 items-center justify-center icons">
        <img src="/question.svg" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.icons {
  img {
    max-width: 100px;
  }
}
@font-face {
  font-family: 'heading';
  src: url('/head-book.ttf');
}
@font-face {
  font-family: 'body-bold';
  src: url('/body-bold.ttf');
}
@font-face {
  font-family: 'body-light';
  src: url('/body-light.ttf');
}
@font-face {
  font-family: 'body-reg';
  src: url('/body-reg.ttf');
}
h1, h2, h3, h4, h5, h6 {
  font-family: 'heading';
}
#investor-relations {
  .hero {
    background-image: url('/Benefits.jpg');
    background-size: cover;
    background-position: center;
    height: 600px;
  }
  .bg-grey {
    background: linear-gradient(to right, #191919, #282828);
  }
  h1 {
    color: white;
    font-size: 80px;
    line-height: 1;
  }
  h3 {
    color: #948477;
    font-size: 20px;
    font-family: "body-bold";
  }
  p {
    color: white;
    font-family: "body-reg";
  }
}
.button {
  font-family: "body-bold";
  font-size: 16px;
  color: #a6a6a6;
  text-transform: uppercase;
  @apply p-4 pr-12 border rounded relative;
  &:after {
  content: url('/Triangle.svg');
    @apply absolute;
    right: 20px;
    top: 50%;
    transform: translateY(-50%);
  }
}
.border-grey {
    border-color: #444444 !important;
}
</style>
