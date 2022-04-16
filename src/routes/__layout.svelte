<script>
  import "../app.css";  
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
</script>
<div class="bg-black h-screen w-screen text-white">
  <Header/>
  
  <slot />
  <Footer/>
</div>