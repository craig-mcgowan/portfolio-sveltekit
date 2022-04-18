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

<form on:submit|preventDefault={handleSubmit} class = "bg-white flex flex-col justify-center text-black w-max shadow rounded-xl py-3 px-8 ">
  <div>
    <label>Name:
      <input type="text" bind:value={formData.name} class="border rounded border-black shadow " />
    </label>
  </div>
  <div>
    <label>Email:
      <input type="email" bind:value={formData.email} class="border rounded border-black shadow "/>
    </label>
  </div>
  <div>
    <label>Message:
      <textarea bind:value={formData.message} class = "border rounded border-black shadow "/>
    </label>
  </div>
  <button type="submit" class= "rounded-lg border-2 border-teal-800 bg-teal-500 text-white h-min px-2 py-1 ">Submit</button>
</form>