     <script>
       import { goto } from "$app/navigation";
     </script>
     
     <header class= "flex w-full justify-between bg-black text-white">
        <div class = "p-2">
            Craig
            McGowan
        </div>
        <nav class="flex justify-around w-max">
          <li class="list-none px-4 py-2" on:click= {()=>goto("/")}>About</li>
          <li class="list-none px-4 py-2"  on:click= {()=>goto("/contact")}>Contact</li>
          <li class="list-none px-4 py-2"  on:click= {()=>goto("/projects")}>Projects</li>
        </nav>
      </header>
