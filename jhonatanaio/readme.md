Este é um projeto que foi desenvolvido ao longo de meses com várias funcionalidades agregadas ao longo do tempo. O programa é utilizado em um raspberry, cada posto de trabalho da fábrica tem uma unidade. O intuito é digitalizar toda a papelada diária dos trabalhadores, criar inovações e automatizar processos. O hardware utilizao é um monitor, mouse, raspberry e um leitor RFID.


É um programa extremamente complexo e robusto, este é o fluxo básico:

-O programa roda em um container Docker em um raspberry

-O fluxo principal acontece no arquivo "ScreenManagement.py", de lá pode-se seguir e analisar classe por classe, função por função

-A tela de login é apresentada 

-O funcionário insere seu crachá no leitor e o login é feito através de leitura RFID "Login_controller.py"

-O funcionário é mantido logado através de uma thread "Login_controller.py" que checa constantemente se o crachá continua inserido

-A tela principal é apresentada Nela estão as funcionalidades principais que podem ser acessadas pelos usuários 

-As funcionalidades são variadas e são desenvolvidas por um outro time interno, o programa somente consome as APIs e exibe as informações
