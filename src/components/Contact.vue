<template>
  <div class="contact">
    <h2>Feel free to contact me <i class="fas fa-paper-plane"></i></h2>
    <a href="mailto: Abdulazizpriv@gmail.com"><p>Abdulazizpriv@gmail.com</p></a>
    <br />
    <p>Copyright 2021 Assao</p>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.contact {
  margin-top: 5rem;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  color: #fff;
  h2 {
    font-size: 3.5rem;
  }
  a {
    color: orange;
    text-decoration: underline;
    font-size: 2rem;
  }
  p {
    padding: 1rem;
  }
}
@media only screen and (max-width: 800px) {
.contact {
  h2 {
    font-size: 2rem;
  }
  a {
    color: orange;
    text-decoration: underline;
    font-size: 1.5rem;
  }
  p {
    padding: 1rem;
  }
}
}
</style>
