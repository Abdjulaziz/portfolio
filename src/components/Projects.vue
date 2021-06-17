<template>
  <div>
    <div class="project-container">
      <div onclick="window.open('https://techon7.dk/', '_blank');" class="projects">
        <img class="logos" src="@/assets/Techon7.svg" alt="" />
        <div class="made-with">
          <h2 class="XD">Adobe XD</h2>
          <h2 class="IA">Illustrator</h2>
          <h2 class="PS">Photoshop</h2>
          <h2 class="ID">Indesign</h2>
        </div>
      </div>
      <div onclick="window.open('https://hayatplakater.dk/', '_blank');" class="projects">
        <img class="logos" src="@/assets/Hayatplakater.svg" alt="" />
        <div class="made-with">
          <h2 class="XD">Adobe XD</h2>
          <h2 class="IA">Illustrator</h2>
          <h2 class="PS">Photoshop</h2>
          <h2 class="VUE">VUE</h2>
        </div>
      </div>
      <div onclick="window.open('https://assao.dk/todolist/', '_blank');" class="projects">
        <i class="fas fa-clipboard-list"></i>
        <div class="made-with">
          <h2 class="VUE">VUE</h2>
        </div>
      </div>
      <div onclick="window.open('https://assao.dk/robotnordic/', '_blank');" class="projects">
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
      <div onclick="window.open('https://assao.dk/matas/', '_blank');" class="projects">
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
  </div>
</template>

<script>
export default {
  name: 'Projects',
};
</script>

<style lang="scss" scoped>
$mainColor: #ffa500;
.container {
  height: 100%;
  width: 100%;
  display: flex;
}
.project-container {
  padding: 5rem 2rem;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-columns: minmax(300px, auto);
  grid-gap: 2rem;
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
}
.made-with {
  padding: 2rem 0;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 1rem;
  font-size: 1rem;
  .HTML {
    padding: 0.5rem;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
    background-color: #e44d26;
    color: #fff;
  }
  .CSS {
    padding: 0.5rem;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
    background-color: #0b74b8;
    color: #fff;
  }
  .JS {
    padding: 0.5rem;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
    background-color: #f7df1e;
    color: #fff;
  }
  .VUE {
    padding: 0.5rem;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
    background-color: #41b883;
    color: #32475b;
  }
  .PS {
    padding: 0.5rem;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
    background-color: #00101c;
    color: #00cafd;
  }
  .XD {
    padding: 0.5rem;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
    background-color: #450135;
    color: #ff60fa;
  }
  .IA {
    padding: 0.5rem;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
    background-color: #330000;
    color: #fe9c00;
  }
  .ID {
    padding: 0.5rem;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
    background-color: #47021e;
    color: #f73163;
  }
}
@media only screen and (max-width: 1660px) {
  .project-container {
    grid-template-columns: repeat(3, 1fr);
    padding: 2rem;
  }
  .made-with {
    grid-template-columns: repeat(3, 1fr);
    font-size: 0.8rem;
  }
}

@media only screen and (max-width: 1190px) {
  .project-container {
    grid-template-columns: repeat(2, 1fr);
  }
  .made-with {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media only screen and (max-width: 800px) {
  .project-container {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>
