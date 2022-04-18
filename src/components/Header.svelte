     <script>
       import { goto } from "$app/navigation";
     </script>
     
     <header class= "flex w-full justify-between bg-black text-white h-12">
        <div class = "p-2">
            <span>Craig</span>
            McGowan
        </div>
        <nav class="flex justify-around w-max">
          <li class="list-none px-4 py-2 hover:text-lg cursor-pointer" on:click= {()=>goto("/")}>About</li>
          <li class="list-none px-4 py-2 hover:text-lg cursor-pointer"  on:click= {()=>goto("/contact")}>Contact</li>
          <li class="list-none px-4 py-2 hover:text-lg cursor-pointer"  on:click= {()=>goto("/projects")}>Projects</li>
        </nav>
      </header>
