
# 🛡️ Pythones

<div class="hacker-console">
Este repositorio centraliza el estudio, práctica y herramientas  
de nuestro equipo para aprender ciberseguridad y  
prepararnos para competencias CTF.
</div>


## 📁 Estructura
- `theory/`: Contenido teórico por categoría (web, crypto, redes...)
- `practice/`: Planes de estudio, ejercicios, plataformas
- `scripts/`: Scripts útiles para automatizar tareas
- `payloads/`: Cheatsheets y comandos rápidos
- `tools/`: Manuales de herramientas comunes
- `notes/`: Apuntes individuales por miembro

## 📚 Cómo contribuir
- Documentar TODO lo que se aprende, incluso errores
- Revisamos cada semana el progreso


<style>
@keyframes flicker {

    0%,
    100% {
        opacity: 1;
    }

    50% {
        opacity: 0.9;
    }
}

@keyframes glitch {

    0%,
    100% {
        clip-path: inset(0 0 0 0);
        transform: translate(0);
        opacity: 1;
    }

    20% {
        clip-path: inset(10% 0 80% 0);
        transform: translate(-1px, -1px);
        opacity: 0.7;
    }

    40% {
        clip-path: inset(80% 0 10% 0);
        transform: translate(1px, 1px);
        opacity: 0.7;
    }

    60% {
        clip-path: inset(10% 0 80% 0);
        transform: translate(-1px, 1px);
        opacity: 0.7;
    }

    80% {
        clip-path: inset(80% 0 10% 0);
        transform: translate(1px, -1px);
        opacity: 0.7;
    }
}

body {
    background-color: #0a0a0a;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
    font-family: 'Courier New', Courier, monospace;
    color: #2ecc71;
}

.hacker-console {
    background: #050805;
    border: 1.5px solid #2ecc71;
    padding: 1.5em 2em;
    width: 600px;
    white-space: pre-wrap;
    position: relative;
    animation: flicker 2s infinite alternate ease-in-out;
    box-shadow: 0 0 6px #2ecc71aa, inset 0 0 6px #2ecc71bb;
    font-size: 18px;
    line-height: 1.4;
    letter-spacing: 0.05em;
}

.hacker-console::before,
.hacker-console::after {
    content: attr(data-text);
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    overflow: hidden;
    color: #2ecc71cc;
    background: transparent;
    mix-blend-mode: screen;
    animation: glitch 3s infinite ease-in-out;
    clip-path: inset(0 0 0 0);
    opacity: 0.6;
    pointer-events: none;
    user-select: none;
    filter: drop-shadow(0 0 1px #2ecc71);
}

.hacker-console::before {
    left: 1px;
    text-shadow: -1px 0 #27ae60;
    animation-delay: 0s;
}

.hacker-console::after {
    left: -1px;
    text-shadow: 1px 0 #16a085;
    animation-delay: 1.5s;
}

</style>
