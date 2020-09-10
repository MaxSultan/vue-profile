<template>
    <div class="nav">
        <div>
            <img src=""/>
            <h1>MaxSULTAN</h1>
        </div>
        <ul class='right'>
            <li class="stack"><a href="" ></a></li>
            <li><a href="" class="linked"><img src=""/>LinkedIn</a></li>
            <li><a href="" class="hub"><img src=""/>Github</a></li>
            <li><a href="" class="pen"><img src=""/>CodePen</a></li>
        </ul>
    </div>    
</template>

<style scoped>
    .nav{
        height: 5em;
        width: 100%;
        background-color: #7FC29E;
        display: flex;
        justify-content:space-between ;
    }
    .right{
        display:flex;
        justify-content: center;
        list-style-type: none;
    }
    li{
        margin: 2rem;
    }
    .stack{
        background: url(../assets/spritesheet.png) no-repeat;
        height: 48px;
        width: 48px;
        background-position: 3000px 2000px;
    }
</style>
