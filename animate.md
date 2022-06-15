

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
body {
 background-image: linear-gradient(to bottom, #152946, #212241, #2b1938, #31102d, #340720);
  font-family: 'Roboto', sans-serif;
  line-height: 1.4;
  padding: 3em 2em;
}

h1 {
  font-weight: 800;
  font-size: 40px;
  text-transform: uppercase;
}

h2 {
  font-weight: 600;
  font-size: 30px;
  text-transform: uppercase;
  width: 100%;
  display: inline;
}

.item {
  margin: 1em 0;
}
.item__number {
  display: inline-block;
  padding: 15px;
  font-size: 34px;
  font-weight: 700;
  width: 45px;
  height: 45px;
  color: #fff;
  border-radius: 50%;
  margin-right: 10px;
  text-align: center;
  z-index: 2;
}
.item__topic {
  padding-left: 80px;
  position: relative;
}
.item__topic:before {
  content: "";
  position: absolute;
  width: 5px;
  height: calc(100% + 1em);
  top: 0;
  left: 35px;
}
.item__topic__title {
  font-weight: 700;
  font-size: 24px;
}
.item__topic__author {
  font-size: 18px;
  color: #999;
}

@media (min-width: 768px) {
  main {
    display: grid;
    max-width: 100%;
    min-height: 150vh;
    padding-bottom: 5em;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: min-content minmax(100px, 0.8fr) repeat(2, 125px) 320px repeat(2, 125px);
  }

  h1 {
    font-size: 50px;
    grid-column: 1/-1;
  }

  .item {
    margin: 0;
  }
  .item:nth-of-type(1) {
    grid-column: 1;
    grid-row: 3;
  }
  .item:nth-of-type(2) {
    grid-column: 2;
    grid-row: 4;
  }
  .item:nth-of-type(3) {
    grid-column: 3;
    grid-row: 3;
  }
  .item:nth-of-type(4) {
    grid-column: 4;
    grid-row: 4;
  }
  .item:nth-of-type(5) {
    grid-column: 1;
    grid-row: 6;
  }
  .item:nth-of-type(5) .item__topic {
    width: 180%;
  }
  .item:nth-of-type(6) {
    grid-column: 2;
    grid-row: 7;
    margin-left: 30%;
  }
  .item:nth-of-type(6) .item__topic {
    width: 200%;
  }
  .item:nth-of-type(7) {
    grid-column: 3;
    grid-row: 6;
    margin-left: 30%;
  }

  .item {
    position: relative;
    text-align: center;
  }
  .item__number {
    font-size: 56px;
    line-height: 1.8;
    width: 95px;
    height: 95px;
    margin: auto;
  }
  .item__topic {
    position: absolute;
    text-align: left;
    width: 130%;
    left: 50%;
    margin-left: -35px;
    padding-left: 60px;
  }
  .item__topic__title {
    margin-bottom: 8px;
  }
  .item--top .item__topic {
    bottom: calc(100% + 1em);
  }
  .item--bottom .item__topic {
    top: 100%;
    padding-top: 10px;
  }
  .item--left .item__topic {
    text-align: right;
    right: 50%;
    left: auto;
    padding-right: 25px;
    width: 140%;
  }
  .item--left .item__topic:before {
    left: auto;
    right: 0;
  }
}
@media (min-width: 1240px) {
  main {
    display: grid;
    margin: auto;
    max-width: 1150px;
    min-height: 120vh;
    grid-template-columns: repeat(4, 125px) 20px repeat(3, 125px) 1fr;
    grid-template-rows: min-content 25% repeat(2, min-content);
    grid-gap: 10px;
  }

  .item:nth-of-type(1) {
    grid-column: 1;
    grid-row: 3;
  }
  .item:nth-of-type(1) .item__topic {
    padding-bottom: 5em;
  }
  .item:nth-of-type(2) {
    grid-column: 2;
    grid-row: 4;
  }
  .item:nth-of-type(2) .item__topic {
    padding-top: 6em;
  }
  .item:nth-of-type(3) {
    grid-column: 3;
    grid-row: 3;
  }
  .item:nth-of-type(3) .item__topic {
    padding-bottom: 11em;
  }
  .item:nth-of-type(4) {
    grid-column: 4;
    grid-row: 4;
    margin-left: 20%;
  }
  .item:nth-of-type(4) .item__topic {
    padding-top: 3em;
    width: 220%;
    margin-right: -16px;
  }
  .item:nth-of-type(5) {
    grid-column: 6;
    grid-row: 3;
  }
  .item:nth-of-type(5) .item__topic {
    padding-bottom: 2em;
  }
  .item:nth-of-type(6) {
    grid-column: 7;
    grid-row: 4;
    margin-left: 15%;
  }
  .item:nth-of-type(6) .item__topic {
    padding-top: 8em;
    left: calc(50% + 7px);
  }
  .item:nth-of-type(7) {
    grid-column: 8;
    grid-row: 3;
  }
  .item:nth-of-type(7) .item__topic {
    padding-bottom: 5em;
    width: 220%;
    left: 70%;
  }
}
.item:nth-of-type(1) .item__number {
  background: rgba(216, 27, 96, 0.6);
}
.item:nth-of-type(1) .item__topic:before {
  background: rgba(216, 27, 96, 0.6);
}
.item:nth-of-type(1) .item__topic__title {
  color: #d81b60;
}
.item:nth-of-type(2) .item__number {
  background: rgba(244, 81, 30, 0.6);
}
.item:nth-of-type(2) .item__topic:before {
  background: rgba(244, 81, 30, 0.6);
}
.item:nth-of-type(2) .item__topic__title {
  color: #f4511e;
}
.item:nth-of-type(3) .item__number {
  background: rgba(58, 61, 183, 0.6);
}
.item:nth-of-type(3) .item__topic:before {
  background: rgba(58, 61, 183, 0.6);
}
.item:nth-of-type(3) .item__topic__title {
  color: #3a3db7;
}
.item:nth-of-type(4) .item__number {
  background: rgba(249, 185, 27, 0.6);
}
.item:nth-of-type(4) .item__topic:before {
  background: rgba(249, 185, 27, 0.6);
}
.item:nth-of-type(4) .item__topic__title {
  color: #f9b91b;
}
.item:nth-of-type(5) .item__number {
  background: rgba(62, 62, 62, 0.6);
}
.item:nth-of-type(5) .item__topic:before {
  background: rgba(62, 62, 62, 0.6);
}
.item:nth-of-type(5) .item__topic__title {
  color: #3e3e3e;
}
.item:nth-of-type(6) .item__number {
  background: rgba(103, 58, 101, 0.6);
}
.item:nth-of-type(6) .item__topic:before {
  background: rgba(103, 58, 101, 0.6);
}
.item:nth-of-type(6) .item__topic__title {
  color: #673a65;
}
.item:nth-of-type(7) .item__number {
  background: rgba(74, 189, 153, 0.6);
}
.item:nth-of-type(7) .item__topic:before {
  background: rgba(74, 189, 153, 0.6);
}
.item:nth-of-type(7) .item__topic__title {
  color: #4abd99;
}

@media (min-width: 1240px) {
  .item {
    overflow: visible;
  }
  .item:before, .item:after {
    content: "";
    position: absolute;
    transform: skew(45deg);
    z-index: -1;
    opacity: 0.3;
  }
  .item:nth-of-type(1):before {
    background: #d81b60;
    width: 120%;
    height: 30px;
    left: 0;
    margin-left: -68%;
    bottom: 25%;
  }
  .item:nth-of-type(1):after {
    background: #673a65;
    width: 40px;
    height: 120%;
    right: 0;
    top: 50%;
  }
  .item:nth-of-type(2):before {
    background: #f4511e;
    width: 35px;
    height: 80%;
    transform: none;
    left: 20%;
    bottom: 38%;
  }
  .item:nth-of-type(2):after {
    background: #f4511e;
    transform: skew(-55deg);
    opacity: 0.5;
    width: 35px;
    height: 25px;
    bottom: 118%;
    left: 35%;
  }
  .item:nth-of-type(3):before {
    background: #3a3db7;
    width: 35px;
    height: 45px;
    transform: none;
    left: -59%;
    bottom: 30%;
  }
  .item:nth-of-type(3):after {
    background: #3a3db7;
    opacity: 0.5;
    width: 108%;
    height: 34px;
    bottom: 40%;
    left: -46%;
  }
  .item:nth-of-type(4):before {
    background: #f9b91b;
    width: 40px;
    height: 120%;
    left: -65%;
    bottom: 55%;
  }
  .item:nth-of-type(4):after {
    background: #4abd99;
    width: 105%;
    height: 30px;
    top: 20%;
    left: -5%;
  }
  .item:nth-of-type(5):before {
    background: #3e3e3e;
    width: 35px;
    transform: none;
    height: 107%;
    left: -49%;
    bottom: -52%;
  }
  .item:nth-of-type(5):after {
    background: #3e3e3e;
    opacity: 0.6;
    width: 72%;
    height: 35px;
    top: 45%;
    left: -35%;
  }
  .item:nth-of-type(6):before {
    background: #673a65;
    width: 40px;
    height: 120%;
    left: -49%;
    top: -63%;
  }
  .item:nth-of-type(6):after {
    background: #4abd99;
    transform: none;
    width: 170%;
    height: 40px;
    bottom: 43%;
    left: 22%;
  }
  .item:nth-of-type(7):before {
    transform: scaleX(-1);
    opacity: 0.5;
    border-left: 35px solid #4abd99;
    border-bottom: 40px solid transparent;
    height: 120px;
    width: 0;
    bottom: -65%;
    left: 18%;
  }
  .item:nth-of-type(7):after {
    top: 37%;
    left: 17%;
    transform: scaleX(-1);
    border-top: 35px solid #3a3db7;
    border-right: 35px solid transparent;
    height: 0;
    width: 295%;
  }
}
    </style>

<main>
  <h1>RoadMap</h1>
  <section>
    <div class="center">
        <h2>TESTE</h1>
    </div>
  </section>
  <div class="item item--top">
    <div class="item__number">1</div>
    <div class="item__topic">
      <div class="item__topic__title">HTML + CSS</div>
      <div class="item__topic__author"> <span></span><span>Gustavo Guanabara</span></div>
    </div>
  </div>
  <div class="item item--bottom item--left">
    <div class="item__number">2</div>
    <div class="item__topic">
      <div class="item__topic__title">Javascript</div>
      <div class="item__topic__author"><span>Gustavo Guanabara</span></div>
    </div>
  </div>
  <div class="item item--top">
    <div class="item__number">3</div>
    <div class="item__topic">
      <div class="item__topic__title">Javascript antes dos frameworks</div>
      <div class="item__topic__author"> <span>Origamid</span></div>
    </div>
  </div>
  <div class="item item--bottom item--left">
    <div class="item__number">+</div>
    <div class="item__topic">
      <div class="item__topic__title">Em breve</div>
      <div class="item__topic__author"> <span></span><span>Mais conteúdos</span></div>
    </div>
  </div>
  <!--
  <div class="item item--top">
    <div class="item__number">5</div>
    <div class="item__topic">
      <div class="item__topic__title">This One Weird Trick Tells Us Everything About You</div>
      <div class="item__topic__author"> <span>by</span><span>Laura Kalbag</span></div>
    </div>
  </div>
  <div class="item item--bottom">
    <div class="item__number">6</div>
    <div class="item__topic">
      <div class="item__topic__title">Quieting Disquiet</div>
      <div class="item__topic__author"> <span>by</span><span>Stuart Langridge</span></div>
    </div>
  </div>
  <div class="item item--top">
    <div class="item__number">7</div>
    <div class="item__topic">
      <div class="item__topic__title">Advertising Is Not  The Problem</div>
      <div class="item__topic__author"> <span>by</span><span>Cennydd Bowles</span></div>
    </div>
  </div>
  -->
</main>