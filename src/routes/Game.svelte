<script>
  import Grid from "./Grid.svelte";
  import {levels} from "../levels.js";


let size: number;
let grid:string[] = [];
let found: string[] = [];

function create_grid(level:Level){

}
</script>
<div class="game">


    <div class="info">

    </div>
    <div class="grid-container">
        <Grid/>
    </div>

    <div class="info">
        
    </div>
</div>

<style>
    .game{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        font-size: min(1vmin, 0.5em);
    }

    .info{
        width: 80vmin;
        height: 10vmin;
        background-color: purple;
    }

    .grid-container{
        display: grid;
  
        width: 80vmin;
        height: 80vmin;
        background-color: teal;
    }
</style>