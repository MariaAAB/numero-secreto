# Numero-Segreto

:video_game: Um jogo para adivinhar qual sera o numero secreto entre 1 a 100 ;
Com apenas uma tentativa , um jogo de Nivel dificil

# Tecnologias :rocket:
 
* HTML ;
* CSS ; 
* Javascript ;
  
:wrench:  Precisaremos ter o Vs Code instalado

:page_facing_up: Aqui teremos as partes mais importes do nosso codigo , essa funcao e resposanvel por gerar o numero aleatorio 


function gerarNumeroAleatorio() {
    let numeroEscolhido = parseInt(Math.random() * numeroLimite + 1);
    let quantidadeDeElementosNaLista = listaDeNumerosSorteados.length;

    if (quantidadeDeElementosNaLista == numeroLimite) {
        listaDeNumerosSorteados = [];
    }
    if (listaDeNumerosSorteados.includes(numeroEscolhido)) {
        return gerarNumeroAleatorio();
    } else {
        listaDeNumerosSorteados.push(numeroEscolhido);
        console.log(listaDeNumerosSorteados)
        return numeroEscolhido;
    }
}


:woman:  Autora : 

  :cherry_blossom: https://github.com/MariaAAB
