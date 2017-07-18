<template lang="html">
  <div>
    <section class="section">
      <div class="columns">

        <div class="column is-1">

        </div>

        <div class="column is-5 has-text-right">
          <span class="title"><strong> Hi , I am a talented software developer from Bangalore</strong></span>
        </div>

        <div class="column is-5">
          <div id="sentence-wrapper">
            <h2 class="sentence">
              <span>You will find me as</span>
              <div class="words words-1">
                <span>Versatile</span>
                <span>Authentic</span>
                <span>Passionate</span>
                <span>Dedicated</span>
                <span>Resourceful</span>
                <span>Learner</span>
                <span>Adaptable</span>
                <span>Ambitious</span>
                <span>Confident</span>
              </div>
            </h2>
          </div>
        </div>

        <div class="column is-1">
        </div>
      </div>
    </section>

    <section class="section">
      <div class="columns">
        <div class="column is-1">

        </div>
        <div class="column">

            <div class="has-text-centered"><i class="fa fa-diamond fa-4x has-text-warning"></i></div>
            <div class="content is-large has-text-centered "><strong>Why Hire Me</strong></div>
            <div class="content">
              I have 3 years of Software Developement experience having performed well wherever I have worked ,
              delivering modules almost always ahead of delivery timelines.
            </div>
            <div class="content">
              I am constantly experimenting, learning and expanding my skills and always being technology agnostic at work.

            </div>
        </div>
        <div class="column">
            <div class="has-text-centered"><i class="fa fa-star fa-4x has-text-warning"></i></div>
            <div class="content is-large has-text-centered"><strong>What I bring to the table</strong></div>
            <div class="content">
              The right attitude to get the job done in the best way possible whether that's by prior knowledge ,
              learning from teammates or finding help on stackoverflow.
            </div>

            <div class="content">
              I am resolute , calm and radiate an aura of reliability in the face
              of strict timelines and pressure situations.
            </div>

        </div>
        <div class="column">
            <div class="has-text-centered"><i class="fa fa-info fa-4x has-text-warning"></i></div>
            <div class="content is-large has-text-centered"><strong>All things personal</strong></div>
            <div class="content">
              Family is the most important thing in life for me , without which the circle is incomplete.
              I love to help out in the family chores. I love to cook.
            </div>

            <div class="content">
              I am a Madridista at heart and watch Real Madrid win with exhuberant jubilation. Rafael Nadal ,
              Raul Gonzalez are two of my biggest inspirations.
            </div>

        </div>
        <div class="column is-1">

        </div>
      </div>
    </section>

    <div class="content is-large has-text-centered is-paddingless">
      <span class="title"><strong>
        Skillset
      </strong></span>
    </div>

    <section class="section">
      <div class="columns">
        <div class="column">
        </div>

        <div class="column  has-text-centered">
          <span class="subtitle"><strong>Getting better day by day</strong></span>
          <table class="table is-striped">
            <tbody>
              <tr>
                <td>HTML / CSS</td>
                <td class="has-text-right">Javascript</td>
              </tr>
              <tr>
                <td>Java</td>
                <td class="has-text-right">Go (Poison of choice)</td>
              </tr>
              <tr>
                <td>Vue JS (Poison of choice)</td>
                <td class="has-text-right">Responsive Design</td>
              </tr>
              <tr>
                <td>Linux (Poison of choice)</td>
                <td class="has-text-right">Git (Poison of choice)</td>
              </tr>
              <tr>
                <td>Flex PLM</td>
                <td class="has-text-right">Windchill</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="column has-text-centered">
          <span class="subtitle"> <strong>I'll find a way </strong></span>
          <table class="table is-striped">
            <tbody>
              <tr>
                <td>AWS</td>
                <td class="has-text-right">Docker</td>
              </tr>
              <tr>
                <td>Chef</td>
                <td class="has-text-right">SQL / No SQL Databases</td>
              </tr>
              <tr>
                <td>React JS</td>
                <td class="has-text-right">Webpack</td>
              </tr>

            </tbody>
          </table>
        </div>
        <div class="column has-text-centered">
          <span class="subtitle"><strong> Things I'm poor at </strong></span>
          <table class="table is-striped">
            <tbody>
              <tr>
                <td class="has-text-centered">Dancing</td>
              </tr>
              <tr>
                <td class="has-text-centered">Singing</td>
              </tr>
              <tr>
                <td class="has-text-centered">Musical Instruments</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="column">
        </div>

      </div>
    </section>
  </div>

</template>

<script>
export default {
  data() {
    return {

    }
  },

  methods : {

  },
}
</script>

<style lang="css">
#sentence-wrapper{
    width: 80%;
    position: relative;
    padding: 10px;
}
.sentence{
    margin: 0;
    text-align: left;
    text-shadow: 1px 1px 1px rgba(255,255,255,0.8);
}
.sentence span{
    color: #444;
    font-size: 200%;
    font-weight: normal;
}
.words{
    display: inline;
    text-indent: 10px;
}
.words-1 span{
    position: absolute;
    opacity: 0;
    overflow: hidden;
    color: #6b969d;
    -webkit-animation: rotateWord 27s linear infinite 0s;
    -moz-animation: rotateWord 27s linear infinite 0s;
    -o-animation: rotateWord 27s linear infinite 0s;
    -ms-animation: rotateWord 27s linear infinite 0s;
    animation: rotateWord 27s linear infinite 0s;
}

.words-1 span:nth-child(2) {
    -webkit-animation-delay: 3s;
    -moz-animation-delay: 3s;
    -o-animation-delay: 3s;
    -ms-animation-delay: 3s;
    animation-delay: 3s;
    color: #6b889d;
}
.words-1 span:nth-child(3) {
    -webkit-animation-delay: 6s;
    -moz-animation-delay: 6s;
    -o-animation-delay: 6s;
    -ms-animation-delay: 6s;
    animation-delay: 6s;
    color: #6b739d;
}
.words-1 span:nth-child(4) {
    -webkit-animation-delay: 9s;
    -moz-animation-delay: 9s;
    -o-animation-delay: 9s;
    -ms-animation-delay: 9s;
    animation-delay: 9s;
    color: #7a6b9d;
}

.words-1 span:nth-child(5) {
    -webkit-animation-delay: 12s;
    -moz-animation-delay: 12s;
    -o-animation-delay: 12s;
    -ms-animation-delay: 12s;
    animation-delay: 12s;
    color: #8d6b9d;
}
.words-1 span:nth-child(6) {
    -webkit-animation-delay: 15s;
    -moz-animation-delay: 15s;
    -o-animation-delay: 15s;
    -ms-animation-delay: 15s;
    animation-delay: 15s;
    color: #9b6b9d;
}
.words-1 span:nth-child(7) {
    -webkit-animation-delay: 18s;
    -moz-animation-delay: 18s;
    -o-animation-delay: 18s;
    -ms-animation-delay: 18s;
    animation-delay: 18s;
    color: #6b889d;
}
.words-1 span:nth-child(8) {
    -webkit-animation-delay: 21s;
    -moz-animation-delay: 21s;
    -o-animation-delay: 21s;
    -ms-animation-delay: 21s;
    animation-delay: 21s;
    color: #6b739d;
}
.words-1 span:nth-child(9) {
    -webkit-animation-delay: 24s;
    -moz-animation-delay: 24s;
    -o-animation-delay: 24s;
    -ms-animation-delay: 24s;
    animation-delay: 24s;
    color: #9b6b9d;
}

@-webkit-keyframes rotateWord {
    0% { opacity: 0; }
    5% { opacity: 0; -webkit-transform: translateY(-30px); }
    7% { opacity: 1; -webkit-transform: translateY(0px);}
    14% { opacity: 1; -webkit-transform: translateY(0px); }
    16% { opacity: 0; -webkit-transform: translateY(30px); }
    80% { opacity: 0; }
    100% { opacity: 0; }
}
@-moz-keyframes rotateWord {
    0% { opacity: 0; }
    5% { opacity: 0; -moz-transform: translateY(-30px); }
    7% { opacity: 1; -moz-transform: translateY(0px);}
    14% { opacity: 1; -moz-transform: translateY(0px); }
    16% { opacity: 0; -moz-transform: translateY(30px); }
    80% { opacity: 0; }
    100% { opacity: 0; }
}
@-o-keyframes rotateWord {
    0% { opacity: 0; }
    5% { opacity: 0; -o-transform: translateY(-30px); }
    7% { opacity: 1; -o-transform: translateY(0px);}
    14% { opacity: 1; -o-transform: translateY(0px); }
    16% { opacity: 0; -o-transform: translateY(30px); }
    80% { opacity: 0; }
    100% { opacity: 0; }
}
@-ms-keyframes rotateWord {
    0% { opacity: 0; }
    5% { opacity: 0; -ms-transform: translateY(-30px); }
    7% { opacity: 1; -ms-transform: translateY(0px);}
    14% { opacity: 1; -ms-transform: translateY(0px); }
    16% { opacity: 0; -ms-transform: translateY(30px); }
    80% { opacity: 0; }
    100% { opacity: 0; }
}
@keyframes rotateWord {
  0% { opacity: 0; }
  5% { opacity: 0; transform: translateY(-30px); }
  7% { opacity: 1; transform: translateY(0px);}
  14% { opacity: 1; transform: translateY(0px); }
  16% { opacity: 0; transform: translateY(30px); }
  80% { opacity: 0; }
  100% { opacity: 0; }
}
</style>
