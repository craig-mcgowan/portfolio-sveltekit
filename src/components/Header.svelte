     <script>
       import { goto } from "$app/navigation";
     </script>
     
     <header>
        <div >
            Craig
            McGowan
        </div>
        <nav>
          <li class="list-none" on:click= {()=>goto("/")}>About</li>
          <li class="list-none"  on:click= {()=>goto("/contact")}>Contact</li>
          <li class="list-none"  on:click= {()=>goto("/projects")}>Projects</li>
  
        </nav>
      </header>
