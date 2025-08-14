let vida = 100;
let forca = 10;

function chooseOption(option){
    const story = document.getElementById("story");

    if(option === "Explorar"){
        story.innerText = "Você encontrou uma floresta sombria... algo se move entre as árvores.";
        
    }
    else if (option === "Lutar"){
        const dano = Math.floor(Math.random()*20);
        vida -= dano;
        story.innerText = `Você enfrentou um inimigo e perdeu ${dano} de vida.`;
    }
    else if (option === "Descansar"){
        vida += 10;
        story.innerText = "Você descansou e recuperou 10 de vida.";
    }

    document.getElementById("vida").innerText = vida;
    document.getElementById("forca").innerText = forca;

    if(vida<=0){
        story.innerText = "Você morreu!☠️ Fim de jogo.";
        document.getElementById("choices").innerHTML = "<button onclick='location.reload()'>Recomeçar</button>";
    }
}
