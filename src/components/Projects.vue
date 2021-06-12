<template>
  <div class="project-container">
    <div class="projects">
      <img class="logos" src="@/assets/Techon7.svg" alt="" />
      <div class="made-with">
        <h2 class="XD">Adobe XD</h2>
        <h2 class="IA">Illustrator</h2>
        <h2 class="PS">Photoshop</h2>
      </div>
    </div>
    <div class="projects">
      <img class="logos" src="@/assets/Hayatplakater.svg" alt="" />
      <div class="made-with">
        <h2 class="XD">Adobe XD</h2>
        <h2 class="IA">Illustrator</h2>
        <h2 class="PS">Photoshop</h2>
        <h2 class="VUE">VUE</h2>
      </div>
    </div>
    <div class="projects">
      <i class="fas fa-clipboard-list"></i>
      <div class="made-with">
        <h2 class="VUE">VUE</h2>
      </div>
    </div>
    <div class="projects">
      <img class="logos" src="@/assets/Robonordic.png" alt="" />
      <div class="made-with">
        <h2 class="XD">Adobe XD</h2>
        <h2 class="IA">Illustrator</h2>
        <h2 class="PS">Photoshop</h2>
        <h2 class="HTML">HTML</h2>
        <h2 class="CSS">CSS</h2>
        <h2 class="JS">JS</h2>
      </div>
    </div>
    <div class="projects">
      <img class="logos" src="@/assets/helsebixen.png" alt="" />
      <div class="made-with">
        <h2 class="XD">Adobe XD</h2>
        <h2 class="IA">Illustrator</h2>
        <h2 class="PS">Photoshop</h2>
        <h2 class="VUE">VUE</h2>
      </div>
    </div>
    <div class="projects">
      <img class="logos" src="@/assets/Matas.svg" alt="" />
      <div class="made-with">
        <h2 class="XD">Adobe XD</h2>
        <h2 class="IA">Illustrator</h2>
        <h2 class="PS">Photoshop</h2>
        <h2 class="HTML">HTML</h2>
        <h2 class="CSS">CSS</h2>
        <h2 class="JS">JS</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Projects',
};
</script>

<style lang="scss" scoped>
$mainColor: #ffa500;
.project-container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: minmax(300px, auto);
  grid-gap: 1rem;
  color: $mainColor;
  background-color: $mainColor;

  .projects {
    color: #fff;
    filter: grayscale(100%);
    cursor: pointer;
    padding: 1rem;
    display: flex;
    justify-content: center;
    flex-direction: column;
    text-align: center;
    background-color: #d8d8d870;
    i {
      font-size: 5rem;
      color: #d8d8d8;
    }
    &:hover {
      filter: grayscale(0%);
      transform: scale(0.9);
      background-color: #002841;
    }
  }
  .logos {
    filter: contrast(200%);
    display: flex;
    justify-content: center;
    align-content: center;
    align-self: center;
    width: 300px;
    max-width: 100%;
    display: block;
    height: auto;
  }
  .made-with {
    padding: 2rem 0;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-auto-rows: minmax(auto, auto);
    grid-gap: 1rem;
    .HTML {
      background-color: #e44d26;
      color: #fff;
    }
    .CSS {
      background-color: #0b74b8;
      color: #fff;
    }
    .JS {
      background-color: #f7df1e;
      color: #fff;
    }
    .VUE {
      background-color: #41b883;
      color: #32475b;
    }
    .PS {
      background-color: #00101c;
      color: #00cafd;
    }
    .XD {
      background-color: #450135;
      color: #ff60fa;
    }
    .IA {
      background-color: #330000;
      color: #fe9c00;
    }
  }
}
@media only screen and (max-width: 1400px) {
  .project-container {
    grid-template-columns: repeat(3, 1fr);
    padding: 2rem;
  }
}
@media only screen and (max-width: 1200px) {
  .project-container {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media only screen and (max-width: 800px) {
  .project-container {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>
