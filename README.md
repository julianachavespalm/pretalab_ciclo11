<h1 align="center">EXERCÍCIO FINAL</h1>

<p align="center"><em>Quadro de Medalhas Olímpico - Implementação em Python</em></p>
<h2>Objetivo</h2>
<p>O programa foi desenvolvido como parte da oficina de seleção do Ciclo Formativo 11 da Pretalab.</p>
<p>O notebook <b>'Exercicio_Final.ipynb'</b> apresenta uma solução em Python para a construção e classificação de um quadro de medalhas olímpico, aderindo aos critérios de desempate estabelecidos pelo Comitê Olímpico Internacional.</p>
<p>O programa coleta e organiza a coleção de medalhas por país, ele apresenta um quadro de medalhas classificado de acordo com os critérios olímpicos:</p>
<ul>
  <li><b>Prioridade 1</b>: classificação pelo maior número de medalhas de ouro. 🥇</li>
  <li><b>Prioridade 2</b>: em caso de empate, classificação pelo maior número de medalhas de prata. 🥈</li>
  <li><b>Prioridade 3</b>: se o empate persistir, classificação pelo maior número de medalhas de bronze. 🥉</li>
</ul>

<h2>Funcionalidades</h2>
<ul>
  <li><b>Coleta de dados:</b> Permite ao usuário inserir o nome do país e a quantidade de medalhas de ouro, prata e bronze conquistadas.</li>
  <li><b>Validação de entrada:</b> Garante que apenas números inteiros sejam aceitos para a quantidade de medalhas, evitando erros no programa.</li>
  <li><b>Classificação:</b> Organiza os países no quadro de medalhas seguindo os critérios olímpicos de desempate.</li>
  <li><b>Exibição de resultados:</b> Apresenta o quadro de medalhas de forma clara, mostrando a posição de cada país, seu nome e a quantidade de medalhas de cada tipo.</li>
</ul>

<h2>Requisitos</h2>
Conta ativa no Google Colab.

<h2>Como rodar</h2>
<ol>
  <li>No navegador, entrar em https://colab.research.google.com/ e realizar login.</li>
  <li>Clicar em "Arquivo".</li>
  <li>Selecionar "Fazer upload de notebook."</li>
  <li>Selecionar a opção "Github".</li>
  <li>No campo "Insira a URL do Github ou pesquise por organização ou usuário", preencher "https://github.com/julianachavespalm/pretalab_ciclo11/"</li>
  <li>Clicar no ícone de lupa 🔍</li>
  <li>Selecionar o notebook "Exercicio_Final.ipynb"</li>
  <li>Ao lado da célula, clicar no botão "Executar célula".</li>
</ol>

<h2>Explicação do código</h2>
<ul>
  <li>Função <b>medalha(tipo_de_medalha)</b>: responsável por coletar e validar a entrada do usuário para o número de medalhas de um tipo específico (ouro, prata ou bronze). Utiliza um loop while True para garantir que o usuário insira um valor numérico válido. Em caso de entrada inválida (ValueError), exibe uma mensagem de erro e solicita novamente a entrada.</li>
  <li>Função <b>obter_criterios_desempate(item)</b>: define os critérios de desempate para a classificação dos países no quadro de medalhas. Retorna uma tupla contendo o número de medalhas de ouro, prata e bronze de um país, nessa ordem de prioridade.</li>
  <li>Função <b>quadro_de_medalhas()</b>: coordena a coleta de dados, a classificação e a exibição do quadro de medalhas. Cria uma lista vazia resultados para armazenar os dados dos países. Utiliza um loop while True para permitir a entrada de dados de vários países até que o usuário digite "sair". Dentro do loop: solicita o nome do país ao usuário; chama a função medalha três vezes para coletar o número de medalhas de ouro, prata e bronze; calcula o total de medalhas somando ouro, prata e bronze; adiciona uma tupla com os dados do país (nome, total de medalhas, ouro, prata, bronze) à lista resultados. Classifica a lista resultados em ordem decrescente usando a função sorted com a chave obter_criterios_desempate. Imprime os critérios de classificação. Itera sobre a lista resultados_ordenados e imprime cada país com sua posição, nome e quantidade de medalhas.</li>
</ul>

<h2>Considerações finais</h2>
<p>O código foi desenvolvido com ênfase na clareza e manutenibilidade, empregando funções para modularizar as responsabilidades e comentários para elucidar a lógica implementada.</p>
<p>A solução apresentada é flexível e adaptável, podendo ser facilmente customizada para contemplar diferentes eventos esportivos ou critérios de classificação específicos.</p>
<p>A utilização do Google Colab proporciona um ambiente de desenvolvimento colaborativo e de fácil acesso para a execução e o compartilhamento do código.</p>

<h2>Autora:</h2> Juliana Chaves Palm
