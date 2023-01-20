<script>
  import svelteLogo from './assets/svelte.svg'
  import Navbar from './lib/Navbar.svelte'
  import Testimonials from './lib/Testimonials.svelte';

    function onTop() {
    window.scrollTo({
        top: 0,
        behavior: 'smooth'
    });
}

let count = 0;

function clickFunc() {
  count += 1;
}

</script>

<main>
  <Navbar />

      <img src={svelteLogo} class="logo svelte" alt="Svelte Logo" />
  <h1>Testimonials with JS Event Listeners! Mouseover = 'paused' while Mouseout = 'running'</h1>

<div class="btncontainer">
  <button on:click={clickFunc}>This button has been clicked {count} times</button>
</div>

<Testimonials />

<h2>Click this illustration to get back on top</h2>

<img src="https://stories.freepiklabs.com/storage/18759/javascript-frameworks-pana-1557.png" class="ill" on:click={onTop} alt="">
    </main>

<style>
main {
  @import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@100;400&display=swap');
  font-family: 'Inter', sans-serif;

}
.logo {
  height: 6vh;
  position: relative;
  top: -7.5vh;
  left: 30vh;
  cursor: pointer;

}

h1 {
  text-align: center;
  margin-top: 4vh;
}

.btncontainer {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}

button {
  background-color: #5f4784;
  height: 50px;
  margin-top: 5vh;
  border-radius: 20px;
  border: 3px solid white;
}

button:hover {
  background-color: rgba(147, 46, 229, 0.4);
  box-shadow: 0px 15px 20px rgba(147, 46, 229, 0.4);
  transform: translateY(-7px);
  transition: 300ms;
  cursor: pointer;
}

h2 {
  margin-top: 20vh;
  text-align: center;
}

.ill {
  display: flex;
  margin: auto;
  cursor: pointer;
}

.ill:hover {
  scale: 1.1;
  transition: 200ms;
}

</style>
