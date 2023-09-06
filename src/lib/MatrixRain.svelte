<script>
    import { onMount } from 'svelte';
  
    onMount(() => {
      const canvas = document.getElementById("matrixCanvas");
      const ctx = canvas.getContext("2d");
  
      canvas.height = window.innerHeight;
      canvas.width = window.innerWidth;
  
      const characters = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789";
      const fontSize = 10;
      const columns = canvas.width / fontSize;
      const drops = [];
      const delays = [];
      const interval = 33;  // Time interval in milliseconds
      let lastTime = 0;
  
      for (let x = 0; x < columns; x++) {
        drops[x] = 1;
        delays[x] = Math.random() * 7000; // Initial delay in milliseconds 
      }
  
      let startTime = null;
  
      function draw(currentTime) {
        if (startTime === null) {
          startTime = currentTime;
        }
        const elapsed = currentTime - startTime;
  
        if (currentTime - lastTime > interval) {
          ctx.fillStyle = "rgba(0, 0, 0, 0.05)";
          ctx.fillRect(0, 0, canvas.width, canvas.height);
  
          ctx.fillStyle = "#0F0";
          ctx.font = fontSize + "px arial";
  
          for (let i = 0; i < drops.length; i++) {
            if (elapsed > delays[i]) {
              const text = characters.charAt(Math.floor(Math.random() * characters.length));
              ctx.fillText(text, i * fontSize, drops[i] * fontSize);
  
              if (drops[i] * fontSize > canvas.height && Math.random() > 0.975) {
                drops[i] = 0;
              }
              
              drops[i]++;
            }
          }
  
          lastTime = currentTime;
        }
  
        requestAnimationFrame(draw);
      }
  
      requestAnimationFrame(draw);
    });
  </script>
  
  <style>
    canvas {
      position: absolute;
      top: 0;
      left: 0;
      z-index: -1;
    }
  </style>
  
  <canvas id="matrixCanvas"></canvas>
  