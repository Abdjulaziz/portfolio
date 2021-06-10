<template>
  <div class="about-section">
    <div class="text">
      <h1>Hello, Im Abdulaziz</h1>
      <h2>
        I <i class="far fa-heart"></i> programming, and like working with front-end and back-end development<br />Programming
        languages iknow.
      </h2>
      <h3>
        C++<br />Python<br />Javascript <br />HTML5 <br />Css3 <br />
        Scss <br />
        Java
      </h3>
      <div class="socials">
        <h2>Catch me here: ↓</h2>
        <a href="https://www.linkedin.com/in/abdulaziz-al-otaibi-0415a6141/" target="_blank"
          ><i class="fab fa-linkedin"></i></a
        ><a href="https://github.com/Abdjulaziz" target="_blank"><i class="fab fa-github-square"></i></a
        ><a href="https://www.artstation.com/onemoretry" target="_blank"><i class="fab fa-artstation"></i></a
        ><a href="https://www.behance.net/abdulazotaibi" target="_blank"><i class="fab fa-behance-square"></i></a>
      </div>
    </div>
    <div class="image">
      <img src="../assets/me.jpg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'About',
};
</script>

<style lang="scss" scoped>
$mainColor: #ffa500;
$secondaryColor: #00568c;
$hoverColor: #fdfffd;
.about-section {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-auto-rows: minmax(700px, auto);
  place-items: center;
  .text {
    padding-left: 3rem;
    border-top: 10px solid $mainColor;
    border-bottom: 10px solid $mainColor;
    display: flex;
    justify-content: center;
    align-content: center;
    flex-direction: column;
    height: 100%;
    width: 100%;
    background-color: $secondaryColor;
    font-size: 1rem;
    color: $mainColor;
    h1,
    h2,
    h3 {
      padding: 1rem;
    }
    .socials {
      i {
        padding: 1rem;
        color: $mainColor;
        font-size: 4rem;
        &:hover {
          color: $hoverColor;
        }
      }
    }
  }
  .image {
    display: flex;
    justify-content: center;
    align-content: center;
    align-self: center;
    align-items: center;
    background-color: $secondaryColor;
    border-top: 10px solid $mainColor;
    border-bottom: 10px solid $mainColor;
    height: 100%;
    width: 100%;
    img {
      max-width: 100%;
      display: block;
      height: auto;
      border-top-left-radius: 100%;
      border-bottom-right-radius: 100%;
      border-bottom-left-radius: 100%;

      &:hover {
        filter: grayscale(100%);
        border-top-left-radius: 0%;
        border-bottom-right-radius: 0%;
        border-bottom-left-radius: 0%;
      }
    }
  }
}
@media only screen and (max-width: 1200px) {
  .about-section {
    grid-template-columns: repeat(1, 1fr);
    place-items: center;
    text-align: center;
  }
}
@media only screen and (max-width: 600px) {
  .about-section {
    .text {
      font-size: 2rem;
    }
  }
}
@media only screen and (max-width: 425px) {
  /*Small smartphones [325px -> 425px]*/
}
</style>
