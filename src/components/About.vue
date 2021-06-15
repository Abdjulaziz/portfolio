<template>
  <div class="about-section">
    <div class="text">
      <h1>Hello, its Abdulaziz here ✌</h1>
      <h2>
        Im a bit of a nerd that likes programming and webdevelopment. Below is some languages that i've worked with.
      </h2>
      <div class="pro-languages">
        <p class="Cpp">#C++</p>
        <p class="Python">#Python</p>
        <p class="Javascript">#Javascript</p>
        <p class="HTML5">#HTML5</p>
        <p class="CSS3">#CSS3</p>
        <p class="SCSS">#SCSS</p>
        <p class="Java">#Java</p>
      </div>
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
$secondaryColor: #002841;
$hoverColor: #fdfffd;
.about-section {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-auto-rows: minmax(700px, auto);
  place-items: center;
  grid-template-areas: 'img', 'txt';
  .text {
    padding-left: 3rem;
    border-top: 10px solid $mainColor;
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
    .pro-languages {
      padding-left: 1rem;
      display: grid;
      grid-template-columns: repeat(3, 100px);
      grid-gap: 5px;
      font-size: 1.2rem;
      color: #ffffff;
      .Cpp {
        display: flex;
        justify-content: center;
        align-content: center;
        border-radius: 5px;
        background-color: #000000;
      }
      .Python {
        display: flex;
        justify-content: center;
        align-content: center;
        border-radius: 5px;
        color: #ffd343;
        background: linear-gradient(#1e415e 10%, #2b5b84 90%);
      }
      .Javascript {
        display: flex;
        justify-content: center;
        align-content: center;
        border-radius: 5px;
        color: #000000;
        background-color: #efd81d;
      }
      .HTML5 {
        display: flex;
        justify-content: center;
        align-content: center;
        border-radius: 5px;
        background-color: #e44d26;
      }
      .CSS3 {
        display: flex;
        justify-content: center;
        align-content: center;
        border-radius: 5px;
        background-color: #1572b6;
      }
      .SCSS {
        display: flex;
        justify-content: center;
        align-content: center;
        border-radius: 5px;
        background-color: #bf4080;
      }
      .Java {
        display: flex;
        justify-content: center;
        align-content: center;
        border-radius: 5px;
        background-color: #c33;
        background: radial-gradient(#c33, #000 99%);
      }
    }
    .socials {
      i {
        padding: 1rem;
        color: #fff;
        font-size: 4rem;
        transition: 1s;
        &:hover {
          color: $mainColor;

          transform: scale(1.2);
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
    .text {
      padding-left: 0rem;
    }
    .pro-languages {
      justify-content: center;
      display: grid;
      grid-template-columns: repeat(3, 100px);
    }
    .image {
      border: 0%;
    } 
  }
}
@media only screen and (max-width: 600px) {
  .about-section {
    .text {
      font-size: 1rem;
    }
  }
}
@media only screen and (max-width: 425px) {
  /*Small smartphones [325px -> 425px]*/
}
</style>
