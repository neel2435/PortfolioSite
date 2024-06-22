<script>
    import MatrixRain from '$lib/MatrixRain.svelte';
    import Titlebar from '$lib/Titlebar.svelte'
</script>
    
<Titlebar />
<MatrixRain />
<body>
    
    <div class = "wrapper">
    <div class="container">
        <div class="about">
            <h1>About Me</h1>
            <p>
                Welcome to my website! I graduated from the 
                <span class="color-blue">University</span>
                <span class="color-yellow">of</span>
                <span class="color-blue">California</span>,
                <span class="color-yellow">Riverside</span> 
                in June 2023 with a degree in Computer Science.
            </p>
            <p>
                I'm looking for careers in the following spaces:
            </p>
            <p class="career">
                Data Analysis/Engineering, 
                Software Engineering/Development, 
                Cybersecurity,
                and 
                Database Administration/Engineering
            </p>
        </div>
    </div>
    </div>
</body>


    
<style>




.wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;

}


.container {
    margin: -5% auto 0;
    padding: 0;
    background: linear-gradient(rgb(26, 29, 27), rgba(110, 211, 144, 1));
    animation: fade-in 1.5s ease forwards;
    border-radius: 20px;
    box-sizing: border-box;
    text-align: center;
    width: 60%;
    max-width: 1400px;
    min-width: 320px; /* Set min-width to a reasonable value */
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
    padding: 2vw; /* Adjust as needed */
    color: white;
    text-align: center; 
    font-family: monospace;
    word-wrap: break-word;
}

h1 {
    font-size: 3vw; /* Adjust as needed */
}

p {
    font-size: 1.5vw; /* Adjust as needed */
    padding: 1vw; /* Adjust as needed */
    margin: 0;
}

p.career {
    font-size: 2vw; /* Adjust as needed */
}

.color-blue {
    color: blue;
}

.color-yellow {
    color: yellow;
}

body {
    background-color: transparent;
    overflow-y: hidden;
    overflow-x: hidden;
}
    
</style>