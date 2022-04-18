<script>
  //import { formData } from "../stores/store.js";
  const formData = {
    name: "",
    email: "",
    message: "",
  };
  const handleSubmit = () => {
    console.log(formData);
    alert("Form submitted");
  }

</script>

Get In Touch with me!

<form on:submit|preventDefault={handleSubmit} class = "bg-white flex flex-column justify-center text-black w-min ">
  <div>
    <label>Name:
      <input type="text" bind:value={formData.name} class="border" />
    </label>
  </div>
  <div>
    <label>Email:
      <input type="email" bind:value={formData.email} class="border"/>
    </label>
  </div>
  <div>
    <label>Message:
      <textarea bind:value={formData.message} class = "border"/>
    </label>
  </div>
  <button type="submit">Submit</button>
</form>