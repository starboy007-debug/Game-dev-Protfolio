<template>
  <div>
    <h1>Resume</h1>

    <div class="paragraph">
      I'm <strong>Pavan Sasane</strong>, from India
      <br />Innovative game programmer and Designer with around 3 years of experience in game development field. 
      Within 3 years of my experience, 
      
      <br />I have created both 2d (Hypercasual and Platformer) and 3d games in Unity game engine
      <br />
      
      <br />Right now I'm working as a solo gamedev 
      <router-link to="/contact">contact me</router-link>.
   
      <br />Besides development, I'm passionate about video games (obviously), and I love cinema, cricket.

      <div style="margin-top:20px; margin-bottom:20px;">
        <a class="download-link" href="d/Pavan.pdf" target="_blank"><i class="fa fa-download fa-lg fa-fw"></i> Download as PDF </a>
        
        <div style="clear:both"></div>
      </div>
    </div>
    <div class="photo">
      <img src="img/PS.ico" alt="Photo of Pavan" />
    </div>

    <div style="clear:both"></div>

    <div class="full-content">
      <h2>Work experience</h2>

      <h3>Unity Game Developer, Ekanomatic V Studio</h3>
      <h4>Jan 2022</h4>

      <div> - Worked on level designing in unity</div>
      <div> - Understood the ongoing project and work on the same project as a game programmer</div>

      <div class="tech-stack">Unity, C#</div>

      <h3>WonderWorld, GGJ + Core Holiday Jam</h3>
      <h4>Dec 2020 - Jan 2021</h4>

      <div> Made 3d survival horror game in worlds largest game creation event taking place around the globe</div>

      <div class="tech-stack">Unity, C#, PhotoShop</div>

      <h2>Skills</h2>

      <div class="skill-set">
        <h3>Languages</h3>
        <SkillRate name="C#" :rate="4" />
        <SkillRate name="Python" :rate="4" />
        <SkillRate name="SQL" :rate="4" />
        <SkillRate name="C++" :rate="4" />
      </div>

      <div class="skill-set">
        <h3>GameDev</h3>
        <SkillRate name="Unity" :rate="4.5" />
        <SkillRate name="Blender" :rate="3" />
        <SkillRate name="Daz3d" :rate="3" />
        <SkillRate name="PhotoShop" :rate="3" />
      </div>

      <div class="skill-set">
        <h3>Tools & Framework</h3>
        <SkillRate name="Visual Studio" :rate="4" />
        <SkillRate name="MakeHuman" :rate="3" />
        <SkillRate name="Git" :rate="4" />
      </div>
      <div style="clear:both" />

      <h2>Education</h2>

      <h3>Engineering - 2023</h3>
      <h4>Comptuer Science engineer</h4>
      <div></div>

      <h2>Languages</h2>

      <h3>English</h3>
    

      <h3>Hindi</h3>


      <h2>Besides...</h2>
      <div>
        <h3>I ❤️ Video games</h3>
        <div>I love playing them, watching them, talking about them, studying them, watching studies about them, designing them...</div>

        <h3>I 🧡 Sports</h3>
        <div>Anything will do but I mainly like Cricket</div>

      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import SkillRate from "@/components/SkillRate.vue";

export default Vue.extend({
  name: "Resume",
  components: {
    SkillRate,
  },
});
</script>

<style scoped>
h2 {
  font-weight: 100;
  font-size: 2em;
  margin: 0px;
  padding: 0px;
  padding-top: 50px;
}
h3 {
  font-weight: 100;
  font-size: 1.6em;
  margin: 0px;
  padding: 0px;
  padding-top: 30px;
}
h4 {
  font-weight: 100;
  font-size: 1.3em;
  margin: 0px;
  padding: 0px;
  padding-top: 15px;
  font-style: italic;
}

.paragraph {
  max-width: 700px;
}

.download-link {
  float:left;
  margin-right: 50px;
}

.full-content div {
  max-width: 800px;
}

.skill-set h3 {
  padding-bottom: 10px;
}

.photo img {
  height: 300px;
  width: 300px;
}

.tech-stack {
  font-style: italic;
}

.photo {
  margin-top: 50px;
  text-align: center;
}

@media only screen and (min-width: 620px){
  .paragraph {
    float: left;
  }

  .photo {
    float: left;
    padding: 30px;
    padding-left: 80px;
  }

  .skill-set {
    float: left;
    padding-right: 60px; 
  }
}
</style>