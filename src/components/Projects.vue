<template>
  <div class="project-container">
    <div class="projects">
      <img class="logos" src="@/assets/Techon7.png" alt="" />
    </div>
    <div class="projects">
      <img class="logos" src="@/assets/Hayatplakater.svg" alt="" />
    </div>
    <div class="projects">
      <i class="fas fa-clipboard-list"></i>
    </div>
    <div class="projects">
      <img class="logos" src="@/assets/Robonordic.png" alt="" />
    </div>
    <div class="projects">
      <img class="logos" src="@/assets/helsebixen.png" alt="" />
    </div>
    <div class="projects">
      <img class="logos" src="@/assets/Matas.svg" alt="" />
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
  padding: 3rem 3rem;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 1rem;
  color: $mainColor;
  .projects {
    cursor: pointer;
    padding: 1rem;
    display: flex;
    justify-content: center;
    flex-direction: column;
    text-align: center;
    border-radius: 5px;
    background-color: #d8d8d8;
    grid-auto-rows: minmax(400px, auto);
    i {
      filter: grayscale(100%);
      font-size: 5rem;
      color: $mainColor;
      &:hover {
        filter: grayscale(0%);
        transform: scale(0.9);
      }
    }
  }
}
.logos {
  filter: grayscale(100%);
  sdisplay: flex;
  justify-content: center;
  align-content: center;
  align-self: center;
  width: 300px;
  max-width: 100%;
  display: block;
  height: auto;
  &:hover {
    filter: grayscale(0%);
    transform: scale(0.9);
  }
}

@media only screen and (max-width: 1200px) {
  .project-container {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media only screen and (max-width: 600px) {
  .project-container {
    grid-template-columns: repeat(1, 1fr);
  }
}
@media only screen and (max-width: 425px) {
  /*Small smartphones [325px -> 425px]*/
}
</style>
