<script>
  import hero_img from "$lib/images/hero_img.webp";
  import devstudio from "$lib/images/devstudio1.png";
</script>

<section class="hero">
  <div class="hero-content">
    <div class="hero-subtitle">
      <h2>Front end Developer</h2>
    </div>
    <h1>Jorge Corzo</h1>
    <p>
      Lorem Ipsum is simply dummy text of the printing and typesetting industry.
      Lorem Ipsum has been the industry's standard dummy text ever since the
      1500s, when an unknown printer took a galley of type and scrambled it to
      make a type specimen book.
    </p>
    <div class="btn">Contact</div>

    <div class="icons"> 
      <img height="50px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain-wordmark.svg" alt="html"/>
      <img height="50px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain-wordmark.svg" alt="css"/>
      <img height="50px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="js"/>
      <img height="50px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" alt="react" />  
      <img height="50px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" alt="node"/>
      <img height="50px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/svelte/svelte-original.svg" alt="svelte"/>
      <img height="50px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original-wordmark.svg" alt="mysql"/>
    </div>
          
  </div>
  <div>
    <img src={hero_img} height="450px"  alt="logo"/>
  </div>
  
</section>

<style>
  .hero {
    display: flex;
    align-items: center;
    justify-content: space-around;
    /* TEMPorary BORDER TO CHECK */
   
  }
  .hero-content {
    text-align: left;
    
  }
  .hero-subtitle {
    width: fit-content;
    padding: 0px 10px 0px 10px;
    border-radius: 5px;
    background-color: var(--colorPrimary);
    color: var(--colorSecundary);
  }
  .hero-subtitle h2 {
    margin-top: 30px;
    margin-bottom: 0;
  }
  .hero-content h1 {
    font-size: 70px;
    margin-top: 0;
    margin-bottom: 0;
  }

  .btn {
    display: inline-block;
    padding: 1rem 2rem;
    background-color: var(--colorPrimary);
    color: var(--colorBackground);
    border-radius: 5px;
    text-decoration: none;
    transition: all 0.3s ease-in;
    margin-bottom: 30px;
  }
  .btn:hover {
    background-color: var(--colorSecundary);
    color: var(--colorPrimary);
  }
  p {
    width: 400px;
    font-style: italic;
    color: gray;
    text-align: start;
  }
  .icons {
    
    margin: 10px;
  }
</style>
