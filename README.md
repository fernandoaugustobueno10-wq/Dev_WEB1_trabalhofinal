Dev_WEB1_trabalhofinal
A Lenda da Digitação — O Portal do Runemestre
Seja bem-vindo a A Lenda da Digitação — O Portal do Runemestre, um jogo em que sua agilidade no teclado se transforma em magia. Aqui, a digitação não é apenas uma mecânica: ela é a sua arma.
Neste universo de RPG medieval, você assume o papel de um Runemestre, um guerreiro das palavras capaz de derrotar inimigos por meio da velocidade e da precisão na digitação. Cada palavra digitada corretamente representa um feitiço lançado, tornando a experiência divertida, desafiadora e educativa ao mesmo tempo.
O projeto foi desenvolvido com o objetivo de unir aprendizado e entretenimento, oferecendo um sistema de progressão individual no Modo Campanha e um ambiente competitivo no Sistema de Ligas, ideal para partidas entre amigos.
Funcionalidades
Sistema de Conta e Progresso
O jogador pode criar uma conta e acessar o sistema por meio de login seguro com uso de password_hash, garantindo maior proteção dos dados. Após entrar no jogo, é possível acompanhar o progresso, visualizar estatísticas e consultar o histórico das partidas.
Modos de Jogo
Modo Campanha
No modo campanha, o jogador enfrenta capítulos com dificuldade progressiva. Durante as batalhas, a vida (HP) é um recurso essencial: erros de digitação reduzem a saúde do personagem, enquanto sequências de acertos (combos) ajudam na recuperação e melhoram o desempenho geral. Ao concluir um capítulo com sucesso, o progresso é salvo automaticamente.
Sistema de Ligas
O sistema de ligas permite criar salas privadas com senha para competir com amigos. Cada liga possui rankings que ajudam a comparar o desempenho dos participantes, tanto de forma geral quanto em períodos específicos.
Mecânicas de Combate
O combate é baseado em velocidade e precisão. O jogador deve digitar corretamente as palavras apresentadas para atacar os inimigos. O sistema de pontuação considera fatores como tempo de resposta e sequência de acertos, incentivando não apenas rapidez, mas também consistência.
Interface e Experiência
A interface do jogo foi construída para ser leve, responsiva e de fácil navegação. Além da ambientação medieval, o projeto conta com efeitos visuais que tornam cada acerto mais satisfatório e reforçam a proposta de transformar a digitação em uma experiência imersiva.
Tecnologias Utilizadas
O projeto foi desenvolvido com uma pilha clássica para aplicações web:

Frontend: HTML, CSS e JavaScript puro
Backend: PHP 7.4+
Banco de Dados: MySQL / MariaDB com PDO
Servidor local recomendado: Apache (XAMPP)

Como Executar o Projeto
Para executar o projeto localmente, é necessário ter um ambiente com servidor web e banco de dados, como XAMPP, WAMP ou LAMP.
Pré-requisitos

PHP 7.4 ou superior
MySQL ou MariaDB
Apache
Navegador atualizado
Ambiente local como XAMPP, WAMP ou LAMP

Passo a passo

Coloque a pasta do projeto dentro do diretório do servidor local. Exemplo no XAMPP:

bashC:\xampp\htdocs\legend-of-typing

Inicie os serviços Apache e MySQL no painel do XAMPP.
Acesse o script de criação do banco de dados no navegador:

http://localhost/legend-of-typing/setup_database.php

Em seguida, execute o script de configuração do sistema de ligas:

http://localhost/legend-of-typing/setup_ligas.php

Caso o MySQL utilize senha, ajuste as credenciais no arquivo config.php.
Por fim, acesse o jogo no navegador:

http://localhost/legend-of-typing/index.php
Como Jogar

Crie sua conta e faça login.
Escolha entre jogar o Modo Campanha ou participar do Sistema de Ligas.
Durante as batalhas:

o inimigo lançará palavras contra você;
digite corretamente e pressione Enter para atacar;
acertos aumentam seus combos e melhoram seu desempenho;
erros reduzem o seu HP.


Sobreviva até o fim do capítulo para salvar sua pontuação e avançar na jornada.
Caso seu HP chegue a zero, a partida termina.

Estrutura do Projeto
A organização principal do código foi dividida da seguinte forma:

index.php — página inicial do sistema
config.php — configuração da conexão com o banco de dados
login.php — autenticação de usuários
register.php — cadastro de novos usuários
logout.php — encerramento de sessão
cap_intro.php — introdução aos capítulos
capitulo.php — lógica principal das batalhas
save_score.php — salvamento de pontuações via AJAX
reset_state.php — reinicialização de estado do jogo
ligas.php — gerenciamento das ligas
liga_ranking.php — ranking das ligas
rankings.php — ranking geral
historico.php — histórico de partidas
setup_database.php — criação do banco e tabelas principais
setup_ligas.php — configuração do sistema de ligas
data/ — arquivos de conteúdo dos capítulos
img/ — imagens e recursos visuais do projeto

Banco de Dados
O sistema utiliza um banco de dados para armazenar as informações principais do jogo, incluindo dados de usuários, pontuações, histórico e ligas.
Entre as tabelas utilizadas, destacam-se:

usuarios
historico_partidas
ligas

Essas tabelas formam a base de persistência do projeto no banco runemestre_db.
Objetivo do Projeto
O principal objetivo deste projeto é transformar a prática da digitação em uma atividade mais interativa, divertida e motivadora. Ao combinar elementos de RPG com mecânicas de precisão e velocidade, o jogo busca estimular o desenvolvimento das habilidades de digitação de forma lúdica.
Além disso, o projeto também serve como aplicação prática de conceitos de desenvolvimento web, integração com banco de dados, autenticação de usuários e manipulação dinâmica de interface.
Melhorias Futuras
Como possíveis evoluções do projeto, destacam-se:

criação de novos capítulos
adição de novos inimigos e desafios
sistema de conquistas
painel administrativo
estatísticas mais detalhadas por jogador
melhorias visuais e sonoras
expansão do sistema competitivo

Autor:
Projeto acadêmico desenvolvido por Fernando Augusto Bueno Canquerini.
