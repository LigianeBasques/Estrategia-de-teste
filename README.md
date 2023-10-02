<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://logowik.com/content/uploads/images/udemy-new-20212512.jpg">
  <source media="(prefers-color-scheme: light)" srcset="https://logowik.com/content/uploads/images/udemy-new-20212512.jpg">
  <img alt="#DescriçãodaImagem:arte gráfica no formato jpg, da logotipo da plataforma de curso Udemy, a cor da letra e preta com acento circunflexo de cor rosa na letra U." src="https://logowik.com/content/uploads/images/udemy-new-20212512.jpg">
</picture>
 
 # 💡Estratégia de teste de software💡 #

 Esse desafio foi proposto em uma live com o seguinte tema : **Pirâmide,** **sorvete** **e** **diamante**: **Como** **e** **onde** **usar?** Do esquenta TDC com cantinho das Qas, ministrado pela mentora **Priscila** **Caimi**. O objetivo é escolher uma funcionaliodade de um site, que utilizamos e aplicar as melhores estratégias de testes no contexto de **Pirâmide** **de** **testes.** 


 ## 🔨Começando o desafio🔨 ##

 O site escolhido para realizar o desafio foi a Udemy que é uma plataforma de aprendizado online que oferece uma ampla variedade de cursos em vídeo sob demanda. O site é https://www.udemy.com/ e a funcionalidade escolhida, foi: "***selecionar*** ***o*** ***curso*** ***e*** ***adicionar*** ***ao*** ***carrinho*** ***de*** ***compras***"

## 🔎Funcionalidade: pesquisar o curso🔎 ## 

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
- [x] 4- Cada resultado da pesquisa deve ser clicável, direcionando-me para a página detalhada do curso correspondente.

### ☑️Definição de Pronto☑️ ###

A funcionalidade de pesquisa de curso na Udemy estará pronta para uso quando todos os critérios de aceitação forem atendidos e a equipe de desenvolvimento e QA estiverem concluído os testes de validação.

### 📝Cenários de testes (CTs)📝 ###

**Funcionalidade:** **Pesquisa de curso na Udemy**
<p><b>CT 0001:</b> Pesquisar por um curso existente</p>
<p><b>Dado</b> que estou na página de cursos da Udemy</p>
<p><b>Quando</b> eu digito "Acessibilidade digital" na barra de pesquisa</p>
<p><b>E</b> pressiono "Enter/Lupa"</p>
<p><b>Então</b> devo ver uma lista de resultados de cursos que contenham "Acessibilidade digital"</p>
<p><b>E</b> cada resultado deve incluir o nome do curso, nome do autor, duração e valor do curso</p>
-----------------------------------------------------------------------------------------------------------------------------------------------

<p><b>CT 0002:</b> Pesquisar por um curso inexistente</p>
<p><b>Dado</b> que estou na página de cursos da Udemy<p>
<p><b>Quando</b> eu insiro "Curso Imaginário" na barra de pesquisa</p>
<p><b>E</b> pressiono "Enter/Lupa"</p>
<p><b>Então</b> devo ver uma mensagem informando que nenhum curso foi encontrado</p>

| ID | Regras |
| ------------- | ------------- |
| [RN-03] |  Deverá conter um botão para adicionar curso no carrinho de compras |
| [RN-04] |  Deverá conter um botão para ir para o carrinho de compras |
| [RN-05] |  Deverá conter um botão para favoritar o curso|
| [RN-05] |  Deverá conter um botão para finalizar compras |
| [RN-06] |  Deverá conter um botão seletor de país |
 

