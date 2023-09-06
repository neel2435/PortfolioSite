<script>
    import MatrixRain from '$lib/MatrixRain.svelte';
    import Titlebar from '$lib/Titlebar.svelte'
</script>
    
<Titlebar />
<MatrixRain />
<body>
    <div class="about">
    
    <h1 style= "font-size: 50px">About Me</h1>
    
    <p style="font-size: 24px; padding: 15px; margin: 0px;">
        Welcome to my website! I graduated from the 
        <span style="color: blue;">University</span>
        <span style="color: yellow;">of</span>
        <span style="color: blue;">California</span>,
        <span style="color: yellow;">Riverside</span> 
        in June 2023 with a degree in Computer Science.<br><br>
        I'm looking for careers in the following spaces:<br><br><br>
    </p>
      
    <p style="
    font-size:35px;
    padding:15px;
    margin:0px;">
    <span style="color: black;">Data</span> 
    Analysis/Engineering, 
    <span style="color: black;">Software</span> 
    Engineering/Development, 
    <span style="color: black;">Cybersecurity</span>,
    and 
    <span style="color: black;">Database</span> 
    Administration/Engineering
    </p>
    
    </div>
</body>
    
<style>
        body {
            position: relative;
            margin: 0 auto;
            top: 200px;
            width: 1400px;
            height: 580px;
            overflow: auto;
            background:linear-gradient(rgb(26, 29, 27), rgba(110, 211, 144, 1));
            opacity: 0;
            animation: fade-in 1.5s ease forwards;
            border-radius: 20px;
            border: 5px solid white;
            box-sizing: border-box;
        }
    
        @keyframes fade-in {
            from {
                opacity: 0; 
                transform: translateY(30%);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    
        .about {
            display: block;
            padding-top: 35px;
            padding-left: 100px;
            padding-right: 100px;
            margin: 0 auto; 
            color: white;
            text-align: center; 
            font-family: monospace;
        }
    
</style>