<h1 align="center"> Subsídios </h1>

<!-- Sobre o projeto -->
## Sobre o projeto 
  O projeto Subsídios é um projeto o qual disponibiliza os relatórios econômicos automatizados. O projeto utiliza dados públicos de comércio do Ministério da Economia e da Onu, também indicadores macroeconômicos publicados pelo Banco Mundial. 
  
## Iniciando 
  Seguem as instruções de como atualizar e gerar os relatórios do comerciobr e comerciomundo. 

## Requisitos 
   Bibliotecas as quais são necessárias para o funcionamento das funções nos gráficos.
   *Observação: Lembrar SEMPRE de conferir pelo menos UM relatório para confirmar se todas as funções estão se portanto normalmente.
   
   install.packages("devtools")
   
   library(devtools)
   
   install.packages("stringr")
   
   library(stringr)
   
   install.packages("stringi")
   
   library(stringi)
   
   install.packages("dplyr")
   
   library(dplyr)

   install.packages("tidyr")
   
   library(tidyr)
  
## Instalação 
   O projeto Subsídios tem como pré-requisito 3 projetos a parte presentes no github da Secretaria de Comércio e Assuntos Econômicos.
   
  *devtools::install_github("NIEscaec/barao2")
  
  *devtools::install_github("NIEscaec/comerciomundo2")
  
  *devtools::install_github("NIEscaec/comerciobr2")
  
   ### A atualização dos dados do comerciobr se consiste em :
    - Abrir o projeto comerciobr.Rproj na pasta do comerciobr2;
    - Na pasta data-raw, abrir o arquivo comextat_dados.R;
    - Rodar TODO o código presente no comextar_dados.R e aguardar ele instalar novamente o pacote. 
    - Caso haja dúvida se os dados estão atualizados, deve se dirigir ao projeto barão e rodar a função comerciobr_get_ultimomes()
  
<!-- Execução -->

## Execução
   Para a execução de todos os relatórios (depois da certeza de que os sub-projetos : barão, comerciobr e comerciomundo) estão atualizados o usuário deve:
   
      - Se dirigir a pasta Subsídios
      - Abrir o projeto subsidios.Rpoj 
      - Na pasta data-raw dentro do subsídios o usuário deve rodar o código do Relatorios.R 
      ⚠️ ATENÇÃO!!! - 
      - Para rodar APENAS os relatórios do comerciobr, rodar o código até o comando "purrr::walk(lista_paises_filtrada, barao2::relatorio_brasil_pais" na linha 16;
      - Para rodar APENAS os relatórios do comerciomundo, rodar apenas o código a partir da linha 17 até o final do código na linha 55.

 ## Visualização 
   Depois de seguir os passos indicados anteriormente, o usuário deve se dirigir a pasta data dentro do projeto subsídios;
   Dentro da pasta data existem duas pastas referentes ao comerciobr e o comerciomundo os quais estão presentes os relatórios de todos os países em suas respectivas pastas 
  
 ## Autores


 [<img src="https://avatars.githubusercontent.com/u/6611471?v=4" width=115><br><sub>Fernando Bastos Neto</sub>](https://github.com/fernandobastosneto)

[<img src="https://avatars.githubusercontent.com/u/87661331?v=4" width=115><br><sub>Henrique Towata Sato</sub>](https://github.com/HenriqueSato) 

  [<img src="https://avatars.githubusercontent.com/u/74457377?v=4" width=115><br><sub>Laura Vieira Fernandes</sub>](https://github.com/l2v6f) 

   [<img src="https://avatars.githubusercontent.com/u/67400736?v=4" width=115><br><sub>Claudio Marconi</sub>](https://github.com/cmarconijr)

  [<img src="https://avatars.githubusercontent.com/u/100308067?v=4" width=115><br><sub>Paulo Victor</sub>](https://github.com/costapaulovictor) 

   [<img src="https://avatars.githubusercontent.com/u/99746076?v=4" width=115><br><sub>Samuel Magalhães </sub>](https://github.com/samuelitamaraty) 


  
