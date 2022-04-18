<script>
  import { goto } from "$app/navigation";
  import ContactLinks from "../components/ContactLinks.svelte";
  import ContactForm from "../components/ContactForm.svelte";
</script>
<div class="flex flex-col content-center items-center">
  <div class = "mb-4">
    <ContactLinks/>
  </div>
  <ContactForm/>
</div>
