# You-are-My-One-Lova
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carta Nocturna</title>
    <link href="https://fonts.googleapis.com/css2?family=Crimson+Pro:wght@400;600&family=Parisienne&display=swap" rel="stylesheet">
    <style>
        body {
            background-color: #2d2d2d;
            font-family: 'Crimson Pro', serif;
            line-height: 1.8;
            margin: 0;
            padding: 20px;
            color: #f0e6d3;
            background-image: 
                linear-gradient(rgba(0,0,0,0.2), rgba(0,0,0,0.2)),
                url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADIAAAAyCAMAAAAp4XiDAAAAUVBMVEWFhYWDg4N3d3dtbW17e3t1dXWBgYGHh4d5eXlzc3OLi4ubm5uVlZWPj4+NjY19fX2JiYl/f39ra2uRkZGZmZlpaWmXl5dvb29xcXGTk5NnZ2c8TV1mAAAAG3RSTlNAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEAvEOwtAAAFVklEQVR4XpWWB67c2BUFb3g557T/hRo9/WUMZHlgr4Bg8Z4qQgQJlHI4A8SzFVrapvmTF9O7dmYRFZ60YiBhJRCgh1FYhiLAmdvX0CzTOpNE77ME0Zty/nWWzchDtiqrmQDeuv3powQ5ta2eN0FY0InkqDD73lT9c9lEzwUNqgFHs9VQce3TVClFCQrSTfOiYkVJQBmpbq2L6iZavPnAPcoU0dSw0SUTqz/GtrGuXfbyyBniKykOWQWGqwwMA7QiYAxi+IlPdqo+hYHnUt5ZPfnsHJyNiDtnpJyayNBkF6cWoYGAMY92U2hXHF/C1M8uP/ZtYdiuj26UdAdQQSXQErwSOMzt/XWRWAz5GuSBIkwG1H3FabJ2OsUOUhGC6tK4EMtJO0ttC6IBD3kM0ve0tJwMdSfjZo+EEISaeTr9P3wYrGjXqyC1krcKdhMpxEnt5JetoulscpyzhXN5FRpuPHvbeQaKxFAEB6EN+cYN6xD7RYGpXpNndMmZgM5Dcs3YSNFDHUo2LGfZuukSWyUYirJAdYbF3MfqEKmjM+I2EfhA94iG3L7uKrR+GdWD73ydlIB+6hgref1QTlmgmbM3/LeX5GI1Ux1RWpgxpLuZ2+I+IjzZ8wqE4nilvQdkUdfhzI5QDWy+kw5Wgg2pGpeEVeCCA7b85BO3F9DzxB3cdqvBzWcmzbyMiqhzuYqtHRVG2y4x+KOlnyqla8AoWWpuBoYRxzXrfKuILl6SfiWCbjxoZJUaCBj1CjH7GIaDbc9kqBY3W/Rgjda1iqQcOJu2WW+76pZC9QG7M00dffe9hNnseupFL53r8F7YHSwJWUKP2q+k7RdsxyOB11n0xtOvnW4irMMFNV4H0uqwS5ExsmP9AxbDTc9JwgneAT5vTiUSm1E7BSflSt3bfa1tv8Di3R8n3Af7MNWzs49hmauE2wP+ttrq+AsWpFG2awvsuOqbipWHgtuvuaAE+A1Z/7gC9hesnr+7wqCwG8c5yAg3AL1fm8T9AZtp/bbJGwl1pNrE7RuOX7PeMRUERVaPpEs+yqeoSmuOlokqw49pgomjLeh7icHNlG19yjsXXK1mL4tuHR8zK53wX/NrlvJLMhZieAAAAAElFTkSuQmCC');
        }
        
        .contenedor {
            max-width: 800px;
            margin: 50px auto;
            padding: 40px;
            background-color: #3a3a3a;
            border-radius: 15px;
            box-shadow: 0 0 30px rgba(0,0,0,0.3);
            border: 1px solid #4a4a4a;
            position: relative;
            overflow: hidden;
        }

        .contenedor::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            right: -50%;
            bottom: -50%;
            background: linear-gradient(45deg, 
                transparent 65%, 
                rgba(230, 57, 80, 0.1) 100%);
            transform: rotate(30deg);
            z-index: 0;
            animation: bg-flow 20s infinite linear;
        }

        .corazon {
            color: #E63950;
            font-size: 40px;
            text-align: center;
            animation: latido 1.5s infinite;
            position: relative;
            z-index: 2;
            text-shadow: 0 0 15px rgba(230, 57, 80, 0.3);
        }
        
        h1 {
            color: #E63950;
            text-align: center;
            font-family: 'Parisienne', cursive;
            font-size: 3em;
            margin: 20px 0;
            text-shadow: 0 0 15px rgba(230, 57, 80, 0.3);
            position: relative;
            z-index: 2;
        }
        
        .fecha {
            text-align: right;
            color: #a8a8a8;
            font-size: 0.95em;
            font-style: italic;
            position: relative;
            z-index: 2;
        }
        
        .poema {
            text-align: center;
            margin: 40px 0;
            padding: 30px;
            background: rgba(0,0,0,0.3);
            border-radius: 8px;
            position: relative;
            z-index: 2;
            border: 1px solid #E63950;
        }
        
        .poema p {
            font-family: 'Crimson Pro', serif;
            color: #f0e6d3;
            font-size: 1.15em;
            line-height: 1.8;
            margin: 25px 0;
            text-shadow: 0 2px 4px rgba(0,0,0,0.2);
        }
        
        .firma {
            font-family: 'Parisienne', cursive;
            font-size: 28px;
            color: #E63950;
            text-align: right;
            margin-top: 40px;
            padding-right: 20px;
            position: relative;
            z-index: 2;
        }
        
        @keyframes latido {
            0% { 
                transform: scale(1); 
                opacity: 0.9;
                text-shadow: 0 0 10px rgba(230, 57, 80, 0.3);
            }
            50% { 
                transform: scale(1.2); 
                opacity: 1;
                text-shadow: 0 0 30px rgba(230, 57, 80, 0.7);
            }
            100% { 
                transform: scale(1); 
                opacity: 0.9;
                text-shadow: 0 0 10px rgba(230, 57, 80, 0.3);
            }
        }

        @keyframes bg-flow {
            0% { transform: rotate(30deg) translateX(-50%); }
            100% { transform: rotate(30deg) translateX(50%); }
        }
        
        .flores {
            text-align: center;
            font-size: 30px;
            margin: 20px 0;
            color: #E63950;
            opacity: 0.7;
            position: relative;
            z-index: 2;
        }
        
        .spotify-player {
            margin: 40px auto;
            max-width: 400px;
            border-radius: 12px;
            overflow: hidden;
            border: 2px solid #E63950;
            box-shadow: 0 0 20px rgba(230, 57, 80, 0.2);
            position: relative;
            z-index: 2;
            background: rgba(0,0,0,0.2);
        }

        ul {
            padding-left: 20px;
            color: #c4c4c4;
            list-style-type: none;
            position: relative;
            z-index: 2;
        }

        ul li {
            margin: 15px 0;
            padding: 12px;
            background: rgba(230, 57, 80, 0.08);
            border-radius: 5px;
            border-left: 3px solid #E63950;
            font-family: 'Crimson Pro', serif;
            transition: transform 0.3s ease;
        }

        ul li:hover {
            transform: translateX(10px);
        }
    </style>
</head>
<body>
    <div class="contenedor">
        <div class="flores">◈ ✦ ◈</div>
        <div class="corazon">♥</div>
        
        <h1>Para Mi Reina de la Noche</h1>
        
        <p class="fecha">8 de Marzo, 2025</p>
        
        <p>Mi Guerrera Oscura,</p>
        
        <p>En este juego de pasiones que nos domina, donde el tiempo se detiene y las calles son nuestro refugio...</p>

        <div class="poema">
            <p>
                "En tus ojos quiero ver historias de nosotros más romanticas que las letras de murder o Gonzalo.<br>
                En cada mirada me vuelves loco y tienes el poder de mirar y yo perderme,<br>
                y en esos labios que me muerden, siento mi realidad vuela<br>
                y el tiempo se rinde ante la intensidad de lo que somos y nos separa sin darnos mas tiempo.
            </p>

            <div class="flores" style="font-size:20px;">⫷⫸</div>

            <p>
                Nuestros atomos vagaron por el universo,<br>
                fueron polvo de estrellas y parte de mundos desconocidos,<br>
                solo para encontrarse en este instante.
            </p>

            <div class="flores" style="font-size:20px;">⫷⫸</div>

            <p>
                Si ya nos veiamos y no nos atrevimos a hablarnos,<br>
                me hace pensar que quizas antes fuimos una sola estrella en el cosmos,<br>
                separada por el tiempo, esperando volver a brillar juntos.
            </p>

            <div class="flores" style="font-size:20px;">⫷⫸</div>

            <p>
                Quiero tomarte fotos todos los dias,<br>
                no solo para recordar lo hermosa que eres,<br>
                sino para capturar cada instante de nuestro amor,<br>
                porque incluso el tiempo merece envidiar nuestro amor.
            </p>
        </div>

        <div class="spotify-player">
            <iframe 
                style="border-radius:12px;" 
                src="https://open.spotify.com/embed/track/1MKsphr9WmAkAGameksHDu?si=pQuLI3ogQ4m-RKsLVRQbUA&theme=0" 
                width="100%" 
                height="152" 
                frameborder="0" 
                allowfullscreen="" 
                allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" 
                loading="lazy">
            </iframe>
        </div>

        <p>Quiero recordarte:</p>
        <ul>
            <li>Que tus ojos son lo mas hermoso</li>
            <li>Que tus abrazos me dan calma</li>
            <li>Que tus besos sin mi vicio</li>
        </ul>
        
        <p>Prometo amarte en cada etapa, celebrar tus logros, apoyarte en los desafíos y construir juntos un futuro donde el amor siga siendo único y envidiable.</p>
        
        <div class="corazon">♥</div>
        <p class="firma">Con todo mi corazón,<br>
        Eazy</p>
        
        <div class="flores">◈ ✦ ◈</div>
    </div>
</body>
</html>