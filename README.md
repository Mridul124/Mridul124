<svg width="300" height="100" viewBox="0 0 300 100" xmlns="http://www.w3.org/2000/svg">
    <style>
        .neon-text {
            font-family: 'Arial', sans-serif;
            font-size: 72px;
            fill: none;
            stroke: #0ff;
            stroke-width: 2;
            stroke-linecap: round;
            stroke-linejoin: round;
            text-anchor: middle;
        }
        
        .neon-text-2 {
            fill: none;
            stroke: #fff;
            stroke-width: 1;
            opacity: 0;
        }
        
        @keyframes neon-flicker {
            0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% {
                opacity: 0.99;
                text-shadow: 
                    0 0 5px #0ff,
                    0 0 10px #0ff,
                    0 0 15px #0ff,
                    0 0 20px #0ff,
                    0 0 25px #0ff,
                    0 0 30px #0ff,
                    0 0 35px #0ff;
            }
            20%, 24%, 55% { 
                opacity: 0.4; 
                text-shadow: none;
            }
        }

        @keyframes neon-glow {
            0%, 100% {
                opacity: 0.9;
                text-shadow: 
                    0 0 5px #0ff,
                    0 0 10px #0ff,
                    0 0 20px #0ff,
                    0 0 30px #0ff,
                    0 0 40px #0ff;
            }
            50% {
                opacity: 0.8;
                text-shadow: 
                    0 0 3px #fff,
                    0 0 5px #fff,
                    0 0 10px #0ff,
                    0 0 15px #0ff;
            }
        }
        
        .neon-text {
            animation: neon-flicker 1.5s infinite alternate;
        }
        
        .neon-text-2 {
            animation: neon-glow 1.5s infinite alternate-reverse;
        }
    </style>
    <text x="50%" y="50%" class="neon-text" dy=".35em">HI</text>
    <text x="50%" y="50%" class="neon-text neon-text-2" dy=".35em">HI</text>
</svg>
