<template>
    <div class="nav">
        <div>
            <img src=""/>
            <h1>MaxSULTAN</h1>
        </div>
        <ul class='right'>
            <li><a href=""><img src=""/>Stack Overflow</a></li>
            <li><a href=""><img src=""/>LinkedIn</a></li>
            <li><a href=""><img src=""/>Github</a></li>
            <li><a href=""><img src=""/>CodePen</a></li>
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
</style>
