 # 💡Estratégia de teste de software💡 #

## 👀Visão Geral👀 ##
Esse desafio foi proposto em uma live com o seguinte tema : **Pirâmide,** **sorvete** **e** **diamante**: **Como** **e** **onde** **usar?** Do esquenta TDC com cantinho das Qas, ministrado pela mentora **Priscila** **Caimi**. O objetivo é escolher uma funcionaliodade de um site, que utilizamos e aplicar as melhores estratégias de testes no contexto de **Pirâmide** **de** **testes**. 

![Ligiabe Basques](https://img.shields.io/badge/Respons%C3%A1vel%3ALigiane%20Basques%20-%20%09%2332CD32)



<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://logowik.com/content/uploads/images/udemy-new-20212512.jpg">
  <source media="(prefers-color-scheme: light)" srcset="https://logowik.com/content/uploads/images/udemy-new-20212512.jpg">
  <img alt="#DescriçãodaImagem:arte gráfica no formato jpg, da logotipo da plataforma de curso Udemy, a cor da letra e preta com acento circunflexo de cor rosa na letra U." src="https://logowik.com/content/uploads/images/udemy-new-20212512.jpg">
</picture>
 
 ## 🔨Começando o desafio🔨 ##

 O site escolhido para realizar o desafio foi a Udemy que é uma plataforma de aprendizado online que oferece uma ampla variedade de cursos em vídeo sob demanda. O site é https://www.udemy.com/ e a funcionalidade escolhida, foi: "***Pesquisar cursos***"

## 🔎Funcionalidade: pesquisar o curso pela barra de pesquisa🔎 ## 
![Barra de pesquisa](https://i.imgur.com/GNqs3bj.png)

### 📋Regras de Negócios (RN)📋 ### 

| ID | Regras |
| ------------- | ------------- |
| [RN-01] |  Deverá conter a barra de pesquisa para: pesquisar o nome do curso ou autor, com até 255 caracteres do tipo string|
| [RN-02] |  Se não houver resultados para a pesquisa, a página deverá exibir uma mensagem informativa: "Infelizmente, não encotramos resultados para tal palavra" |
| [RN-03] | A pesquisa deve ser sensível a maiúsculas e minúsculas, garantindo que se possa encontrar cursos independentemente da capitalização das palavras-chave. |

### 🎯User Story (US)🎯 ###

<p> <b>Como</b> um usuário da plataforma Udemy </p> 
<p> <b>Gostaria</b> de realizar uma pesquisa por nome do curso ou autor, na página de cursos da Udemy </p>
<p> <b>Para</b> encontrar rapidamente o curso específico que estou procurando</p>

### ✅Critérios de aceite✅ ####

- [x] 1- Na página de cursos da Udemy, deve haver uma barra de pesquisa visível na parte superior da página;
- [x] 2- O campo de pesquisa deve ser de fácil acesso e claramente identificável para os usuários;
- [x] 3- Quando eu digitar o nome ou parte do nome de um curso no campo de pesquisa e pressionar "Enter" ou clicar no botão da "lupa", a página deverá mostrar resultados correspondentes à minha pesquisa;
- [x] 4- Cada resultado da pesquisa deve ser clicável, direcionando-me para a página detalhada do curso correspondente;
- [ ] 5- Ao pesquisar um curso, quero poder adicioná-lo ao meu carrinho de compras,favoritá-lo para uma possível compra futura ou comprá-lo agora.

### ☑️Definição de Pronto☑️ ###

A funcionalidade de pesquisa de curso na Udemy estará pronta para uso quando todos os critérios de aceitação forem atendidos e a equipe de desenvolvimento e QA estiverem concluído os testes de validação.

### 📝Cenários de testes (CTs)📝 ###

**Funcionalidade:** **Pesquisar curso na Udemy na barra de pesquisa**
<p><b>CT 0001:</b> Pesquisar por um curso existente</p>
<p><b>Dado</b> que estou na página de cursos da Udemy</p>
<p><b>Quando</b> eu digito "Acessibilidade digital" na barra de pesquisa</p>
<p><b>E</b> pressiono "Enter/Lupa"</p>
<p><b>Então</b> devo ver uma lista de resultados de cursos que contenham "Acessibilidade digital"</p>
<p><b>E</b> cada resultado deve incluir o nome do curso, nome do autor, duração e valor do curso</p>
-----------------------------------------------------------------------------------------------------------------------------

<p><b>CT 0002:</b> Pesquisar por um curso inexistente</p>
<p><b>Dado</b> que estou na página de cursos da Udemy<p>
<p><b>Quando</b> eu digito "Curso Imaginário" na barra de pesquisa</p>
<p><b>E</b> pressiono "Enter/Lupa"</p>
<p><b>Então</b> devo ver uma mensagem informando que nenhum curso foi encontrado</p>
-----------------------------------------------------------------------------------------------------------------------------

<p><b>CT 0003:</b> Pesquisar por um curso com letras maiúsculas e minúsculas</p>
<p><b>Dado</b> que estou na página de cursos da Udemy</p>
<p><b>Quando</b> eu digito "acessibilidade digital/ACESSIBILIDADE DIGITAL" na barra de pesquisa</p>
<p><b>E</b> pressiono "Enter/Lupa"</p>
<p><b>Então</b> devo ver uma lista de resultados de cursos que contenham "Acessibilidade digital"</p>
<p><b>E</b> a pesquisa deve ser sensível a letras maiúsculas e minúsculas</p>
-----------------------------------------------------------------------------------------------------------------------------

<p><b>CT 0004: </b>Clicar em um resultado de pesquisa</p>
<p><b>Dado</b> que estou na página de resultados de pesquisa da Udemy</p>
<p><b>Quando</b> eu clico no primeiro resultado da lista</p>
<p><b>Então</b> devo ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

## 🔎Funcionalidade: pesquisar o curso por categoria🔎 ## 
![Pesquisa cursos por filtros](https://i.imgur.com/Rq17khJ.png)

### 📋Regras de Negócios (RN)📋 ### 

| ID | Regras |
| ------------- | ------------- |
| [RN-04] |  Deverá conter um botão link âncora: "Desenvolvimento" para direcionar para seções: "Desenvolvimento web", "Linguagens de programação", "Desenvolvimento de games", "Design e desenvolvimento de bancos de dados" e "Teste de software"  |
| [RN-05] |  Deverá conter um botão link âncora: "Negócios" para direcionar para seção: "Emprededorismo", "Comunicação", "Administração", "Vendas"e  "Estratégias de negócios" |
| [RN-06] |  Deverá conter um botão link âncora: "Finanças e contabilidade" para direcionar para seção: "Contabilidade e escrituração contábil", "Criptomoeda e blockchain", "Finanças", "Modelagem e análise financeira" e "Investimentos e trading "|
| [RN-07] |  Deverá conter um botão link âncora: "TI e software" para direcionar para seção: "Certificações de TI", "Rede e segurança", "Hardware", "Sistema operacionais e servidores" e "Mais opções em Ti e software" |
| [RN-08] |  Deverá conter um botão link âncora: "Produtividade no escritório" para direcionar para seção: "Microsoft", "Apple","Google", "SAP", "Oracle" e "Mais opções em produtividade no escritório"|
| [RN-09] |  Deverá conter um botão link âncora: "Desenvolvimento Pessol" para direcionar para seção: "Transformação pessoal","Produtividade pessoal", "Liderança", "Desenvolvimento de carreira" e "Maternidade/paternidade e relacionamentos" |
| [RN-10] |  Deverá conter um botão link âncora: "Desenvolvimento Pessol" para direcionar para seção: "Web design","Designe gráfico e ilustração", "Ferramentas de design", "Design de experi^ncia do usuário","Design de games" e "3D e animação" |

### 🎯User Story (US)🎯 ###

<p> <b>Como</b> um usuário da plataforma Udemy </p> 
<p> <b>Gostaria</b> de realizar uma pesquisa refinada de cursos usando categorias </p>
<p> <b>Para</b> encontrar cursos que atendam especificamente às minhas necessidades e interesses.</p>

### ✅Critérios de aceite✅ ####

- [x] 1- Como usuário logado na Udemy, desejo acessar a função de pesquisa por categoria no site;
- [ ] 2- Na página de pesquisa de cursos, quero ver uma variedade de categorias disponíveis,incluindo as categorias: "Desenvolvimento","Negócios", "Finanças e contabilidade","TI e software","Produtividade no escritório", "Desenvolvimento Pessol" e "Design de games";
- [ ] 3- Ao aplicar categoria por exemplo: "Desenvolvimento", desejo ver a lista de cursos atualizada automaticamente para exibir apenas os cursos que correspondem a essa categoria;
- [ ] 4- Ao clicar em um curso da lista de resultados, desejo ser direcionado para a página do curso, onde posso ver informações detalhadas sobre o curso, como descrição, grade curricular, valor, nome do autor e análises de outros alunos;
- [ ] 5- Ao escolher um curso, quero poder adicioná-lo ao meu carrinho de compras,favoritá-lo para uma possível compra futura ou comprá-lo agora.

### ☑️Definição de Pronto☑️ ###

A funcionalidade de pesquisar curso por categoria na Udemy estará pronta para uso quando todos os critérios de aceitação forem atendidos e a equipe de desenvolvimento e QA estiverem concluído os testes de validação.

### 📝Cenários de testes (CTs)📝 ###

**Funcionalidade:** **Verificação do botão link âncora "Desenvolvimento" e suas seções**
<p><b>CT 0005:</b> Clicar no link âncora "Desenvolvimento" e direcionar para as seções</p>
<p><b>Dado</b> que o usuário está na página principal de cursos da Udemy"</p>
<p><b>Quando</b> o usuário clica no link âncora "Desenvolvimento"</p>
<p><b>Então</b> o usuário deve ser redirecionado para a seção "Desenvolvimento web" por exemplo</p>
<p><b>E</b> o usuário ao clicar em "Desenvolvimento web" deverá ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

**Funcionalidade:** **Verificação do botão link âncora "Negócios" e suas seções**
<p><b>CT 0006:</b> Clicar no link âncora "Negócios" e direcionar para as seções</p>
<p><b>Dado</b> que o usuário está na página principal de cursos da Udemy"</p>
<p><b>Quando</b> o usuário clica no link âncora "Negócios"</p>
<p><b>Então</b> o usuário deve ser redirecionado para a seção "Emprededorismo" por exemplo</p>
<p><b>E</b> o usuário ao clicar em "Emprededorismo" deverá ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

**Funcionalidade:** **Verificação do botão link âncora "Finanças e contabilidade" e suas seções**
<p><b>CT 0007:</b> Clicar no link âncora "Finanças e contabilidade" e direcionar para as seções</p>
<p><b>Dado</b> que o usuário está na página principal de cursos da Udemy"</p>
<p><b>Quando</b> o usuário clica no link âncora "Finanças e contabilidade"</p>
<p><b>Então</b> o usuário deve ser redirecionado para a seção "Contabilidade e escrituração contábel" por exemplo</p>
<p><b>E</b> o usuário ao clicar em "Contabilidade e escrituração contábel" deverá ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

**Funcionalidade:** **Verificação do botão link âncora "TI e software" e suas seções**
<p><b>CT 0008:</b> Clicar no link âncora "TI e software" e direcionar para as seções</p>
<p><b>Dado</b> que o usuário está na página principal de cursos da Udemy"</p>
<p><b>Quando</b> o usuário clica no link âncora "TI e software"</p>
<p><b>Então</b> o usuário deve ser redirecionado para a seção "Certificações de TI" por exemplo</p>
<p><b>E</b> o usuário ao clicar em "Certificações de TI" deverá ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

**Funcionalidade:** **Verificação do botão link âncora "Produtividade no escritório" e suas seções**
<p><b>CT 0009:</b> Clicar no link âncora "Produtividade no escritório" e direcionar para as seções</p>
<p><b>Dado</b> que o usuário está na página principal de cursos da Udemy"</p>
<p><b>Quando</b> o usuário clica no link âncora "Produtividade no escritório"</p>
<p><b>Então</b> o usuário deve ser redirecionado para a seção "Microsoft" por exemplo</p>
<p><b>E</b> o usuário ao clicar em "Microsoft" deverá ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

**Funcionalidade:** **Verificação do botão link âncora "Desenvolvimento Pessoal" e suas seções**
<p><b>CT 0010:</b> Clicar no link âncora "Desenvolvimento Pessoal" e direcionar para as seções</p>
<p><b>Dado</b> que o usuário está na página principal de cursos da Udemy"</p>
<p><b>Quando</b> o usuário clica no link âncora "Desenvolvimento Pessoal"</p>
<p><b>Então</b> o usuário deve ser redirecionado para a seção "Transformação pessoal" por exemplo</p>
<p><b>E</b> o usuário ao clicar em "Transformação pessoal" deverá ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

**Funcionalidade:** **Verificação do botão link âncora "Design" e suas seções**
<p><b>CT 0011:</b> Clicar no link âncora "Design" e direcionar para as seções</p>
<p><b>Dado</b> que o usuário está na página principal de cursos da Udemy"</p>
<p><b>Quando</b> o usuário clica no link âncora "Designl"</p>
<p><b>Então</b> o usuário deve ser redirecionado para a seção "Web design" por exemplo</p>
<p><b>E</b> o usuário ao clicar em "Web design" deverá ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

**Funcionalidade:** **Verificação do botão link âncora "Marketing" e suas seções**
<p><b>CT 0012:</b> Clicar no link âncora "Marketing" e direcionar para as seções</p>
<p><b>Dado</b> que o usuário está na página principal de cursos da Udemy"</p>
<p><b>Quando</b> o usuário clica no link âncora "Marketing"</p>
<p><b>Então</b> o usuário deve ser redirecionado para a seção "Marketing digital" por exemplo</p>
<p><b>E</b> o usuário ao clicar em "Marketing digital" deverá ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

**Funcionalidade:** **Verificação do botão link âncora "Saúde e fitness" e suas seções**
<p><b>CT 0013:</b> Clicar no link âncora "Saúde e fitness" e direcionar para as seções</p>
<p><b>Dado</b> que o usuário está na página principal de cursos da Udemy"</p>
<p><b>Quando</b> o usuário clica no link âncora "Saúde e fitness"</p>
<p><b>Então</b> o usuário deve ser redirecionado para a seção "Fitness" por exemplo</p>
<p><b>E</b> o usuário ao clicar em "Fitness" deverá ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

**Funcionalidade:** **Verificação do botão link âncora "Música" e suas seções**
<p><b>CT 0014:</b> Clicar no link âncora "Música" e direcionar para as seções</p>
<p><b>Dado</b> que o usuário está na página principal de cursos da Udemy"</p>
<p><b>Quando</b> o usuário clica no link âncora "Música"</p>
<p><b>Então</b> o usuário deve ser redirecionado para a seção "Instrumentos" por exemplo</p>
<p><b>E</b> o usuário ao clicar em "Instrumentos" deverá ser redirecionado para a página detalhada desse curso</p>
-----------------------------------------------------------------------------------------------------------------------------

### ✅Aplicando a estratégia da pirâmide de testes✅ ###

![Pirâmide de testes](https://i.imgur.com/8X4M3SL.png) 
**Fonte: Priscila Caimi**
<p>A pirâmide de testes ajuda as equipes de desenvolvimento a priorizarem onde colocar esforços de testes e a construir um conjunto de testes robusto que ajude a garantir a qualidade do software ao longo de todo o ciclo de desenvolvimento: a seguir, será demostrado onde cada teste deverá se aplicado em se tratando desse modelo.  </p>

![Static Badge](https://img.shields.io/badge/Unit%C3%A1rio-FF0000?style=flat)

 **Regras de Negócios (RN)**
<p>Será validado no teste unitário as regras de negócios, que no exemplo acima se trata da: funcionalidade de pesquisar os cursos na barra de pesquisa e através de categórias. </p>









 
 

