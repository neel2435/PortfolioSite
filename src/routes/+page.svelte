<script>
    import MatrixRain from '$lib/MatrixRain.svelte';
    import Titlebar from '$lib/Titlebar.svelte'
</script>

<Titlebar />
<MatrixRain />
<body>
    <div class = "typewriter1">
       Hey, I'm Neel
    </div>  
    <div class = "typewriter2">
        University of California, Riverside
    </div>
    <div class = "typewriter3">
        Computer Science with Business Applications
    </div>
</body>

<style>
    
    body {
        /* height: 935px; */
        background:linear-gradient(rgba(0, 0, 0, 0.35), rgba(0, 0, 0, 0.35));
    }

    .typewriter1 {
        color: white;
        justify-content: center;
        text-align: center;
        position: absolute;
        place-items: center;
        top: 40%;
        left: 50%;
        transform: translate(-50%, -50%);
        animation: typing1 1s steps(22) forwards, blink .5s step-end infinite alternate;
        white-space: nowrap;
        overflow: hidden;
        border-right: 3px solid;
        font-family: monospace;
        font-size: 2.73vw;
        padding: 0px;
    }

    .typewriter2{
        color: white;
        justify-content: center;
        text-align: center;
        position: absolute;
        place-items: center;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        animation: typing2 1s 1s steps(22) both, blink .5s step-end infinite alternate;
        white-space: nowrap;
        overflow: hidden;
        border-right: 3px solid;
        font-family: monospace;
        font-size: 1.37vw;
        padding: 0px;
        display: inline-block;
    }

    .typewriter3{
        color: white;
        justify-content: center;
        text-align: center;
        position: absolute;
        place-items: center;
        top: 55%;
        left: 50%;
        transform: translate(-50%, -50%);
        animation: typing3 1s 2s steps(22) both, blink .5s step-end infinite alternate;
        white-space: nowrap;
        overflow: hidden;
        border-right: 3px solid;
        font-family: monospace;
        font-size: 1.03vw;
        padding: 0px;
        display: inline-block;
    }

    @keyframes typing1 {
        from { width: 0 }
        to { width: 19.5% }
    }
           
    @keyframes typing2 {
        from { width: 0 }
        to { width: 26.5% }
    }

    @keyframes typing3 {
        from { width: 0 }
        to { width: 24.5% }
    }

    @keyframes blink {
        50% {
            border-color: transparent
        }
    }

</style>