# Dashboard-SAGEP

## Sobre o Projeto

Este projeto consiste em uma automação para a criação de um dashboard desenvolvido no Power BI com o objetivo de analisar a situação dos protocolos que circulam a Secretaria Adjunta de Gestão de Pessoas(SAGEP), um setor da Secretaria de Estado de Educação do Pará (SEDUC).

## Principais Funcionalidades

- **Consulta Processos:** O bot irá entrar na pasta "Entrada da Unidade" e realizará uma varredura da pasta "PROCESSO JUDICIAL", gerando no final uma planilha para consulta individual de cada protocolo, a partir desta planilha o bot irá consultar cada nº de protocolo presente nela, nos gerando uma nova planilha apenas com as informações que iremos utilizar para a criação do dashboard.

  - **Tratamento das Planilhas:** Um script feito para tratar as planilhas geradas na consulta dos processos, editando as mesmas para nos retornar apenas as informações que serão utilizadas no dashboard final.
 
  - **Tempo Médio de Resposta:**
