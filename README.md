# Sistemas de Apostas Futebol - BET 
(TRABALHO UNIVERSITÁRIO - IFPI)

# Descrição:
Plataforma que permite usuários realizarem apostas sobre os resultados de Partidas de Futebol. Todos os jogos de quaisquer campeonatos ou países podem ser incluídos no sistema.

A título de informação uma partida de de futebol é:
* Pertence a um campeonato de abrangência qualquer: Estadual, Nacional, Continental ou mundial;
* Realizada entre dois times ou seleções, sendo sempre um o mandante do jogo, dito CASA e o outro visitante, chamado FORA;
* O resultado da partida a ser considerado é do tempo normal  (90min mais acréscimos).
* O resultado é informado na forma de Placar, e ainda uma situação descritiva, tais como: EMPATE, CASA GANHA, FORA GANHA
* Ocorre em um local e data/hora

* Times e campeonatos podem receber siglas para facilidade de uso do sistema. (Ex.: Flamengo -> FLA, Copa do Nordeste -> CNE)

* Os usuários podem realizar apostas em qualquer jogo ainda não iniciado. 

* Um bilhete custa R$ C e é composto de N apostas, cada uma sobre uma partida

* Cada aposta deve indicar a situação descritiva para a sua Partida

* Não se pode incluir uma mesma partida mais de uma vez no mesmo bilhete.

* Cada bilhete recebe um identificador único na plataforma

* Cada bilhete recebe um usuário (logado) como o apostador.

A plataforma funciona em fluxo contínuo. Sendo verificados os bilhetes à medida que a rodada que possui os jogos ali especificados, seja finalizada:
* Um bilhete é dito PREMIADO se todas as N apostas que o compõe estiverem marcadas como ACERTOU. 
* A plataforma retém 20% do valor arrecadado;
* Os 80% demais são distribuídos entre os acertadores, se houver.

[Detalhe de implementação*] Regra inicial de distribuição dos prêmios: O valor a ser pago por um bilhete premiado é calculado a partir das apostas certas. Cada aposta do bilhete leva sua cota(entre os acertadores) dos 80%. Só entra no rateios as apostas de bilhetes premiados.

*Ex.: Um bilhete premiado(custo de R$ 5), ou seja acertou todas as 5 apostas, terá seu valor calculado em cada aposta, seja a aposta n1, da partida  Flamengo x River no Rio-RJ, CASA GANHA, que foi incluída em 1200 bilhetes, portanto tem 80% (R$ 960) para ser rateado entre os 71 bilhetes premiados que incluíram essa partida, ou seja, essa aposta contribuiu para o prêmio/bilhete de cada apostador com (960/71) R$ 13,52. Assim o prêmio do bilhete é a soma das cotas de cada aposta.*
