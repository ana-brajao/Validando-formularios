<p align="center">Formulário de criação de contas para o banco virtual MoniBank.</p>

## Implementar validações nos campos do formulário de cadastro do Monibank.

Para isso acessei a página do projeto rodando em tempo real disponível neste link onde encontrei as páginas de funcionamento da aplicação a fim de entender o que precisamos desenvolver. Na tela "Abrir conta" temos a primeira parte do formulário.

O campo "Nome" possui duas mensagens de verificação que são ativadas através das situações abaixo:

Se clicar no campo e em seguida clicarmos fora dele, a mensagem "O campo de nome não pode estar vazio." é exibida;
Se clicar no campo, e digitar alguns caracteres antes de clicar fora dele, a mensagem "Por favor, preencha um nome válido." será exibida.
Perceba que o sistema possui várias mensagens customizadas para cada tipo de erro que pode ocorrer. Vou implementá-las em todos os campos dessa página.

Em seguida, como bônus, implementei a página de reconhecimento facial do nosso formulário, disponível para consulta neste link. Nela a pessoa usuária será capaz de capturar uma imagem sua com a câmera — ou seja, aprender a tirar fotografias com Javascript!
Ao clicar no quadro será exibida a imagem da nossa câmera e um botão com o texto "Tirar foto". Se clicar no botão, a foto será tirada e ficará salva na tela. Abaixo da foto, será exibido um ícone de "check" (ou verificação) redondo junto à mensagem "Prontinho, imagem capturada!". Abaixo dessa mensagem será exibido um botão com o texto "Quero abrir minha conta!".

Para implementar tudo isso será abordado os tópicos:

Atributos do HTML5, como:

Required que torna o campo obrigatório;

Type que define o tipo de input;

min-length e max-length que controlam a quantidade de caracteres do input e

pattern que deve ser implementado no interior de regexs (expressões regulares, em português);

Ferramentas do Javascript, como:

addEventListener que detecta interações da pessoa usuária com o cadastro;

verificação de CPF que possuirá uma lógica para validar os seus dois últimos dígitos;

verificação de maioridade já que o Monibank não aceita menores de idade abrindo contas;

ValidityState para verificar os erros que ocorrem no preenchimento do elemento;

manipulação de DOM para imprimir mensagens de erro.

localStorage para salvar os dados. Mesmo que nosso formulário seja local, é necessário que suas informações sejam salvas em um local específico.


Um pouco de HTML e CSS, pois não construiremos essa parte no projeto — implementaremos códigos HTML e CSS já prontos.
Conhecer essas validações é essencial, pois podem ser aplicadas em qualquer aplicação que possua um formulário — seja para criação de contas em e-commerce e até mesmo em contas de redes sociais.

## Tecnologias utilizadas no projeto
* HTML
* CSS
* JavaScript
Javascript assíncrono;
Manipulação de DOM;
localStorage;
