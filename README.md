# Dashboard-SAGEP

## Sobre o Projeto

Este projeto consiste em uma automação para a criação de um dashboard desenvolvido no Power BI com o objetivo de analisar a situação dos protocolos que circulam a Secretaria Adjunta de Gestão de Pessoas(SAGEP), um setor da Secretaria de Estado de Educação do Pará (SEDUC).

## Principais Funcionalidades

- **Consulta processos:** O bot irá entrar na pasta "Entrada da Unidade" e realizará uma varredura da pasta "PROCESSO JUDICIAL", gerando no final uma planilha para consulta individual de cada protocolo, a partir desta planilha o bot irá consultar cada nº de protocolo presente nela, nos gerando uma nova planilha apenas com as informações que iremos utilizar para a criação do dashboard.

  - **Tratamento das planilhas:** Um script feito para tratar as planilhas geradas na consulta dos processos, editando as mesmas para nos retornar apenas as informações que serão utilizadas no dashboard final.
 
  - **Tempo médio de resposta:** Gráfico de barras empilhadas que calcula a média do tempo de resposta em dias em que cada setor da SAGEP demora para encaminhar um processo.
 
  - **Resposta total SAGEP:** Gráfico de colunas empilhadas que retorna intervalo de dias em que um processe é respondido dentro da SAGEP, indo de 0 até maior ou igual a 5 dias, o resultado é mostrado em porcentagem.
 
  - **Processo mais antigo por setor:** Gráfico de barras empilhadas que retorna o(s) processo(s) que estão a mais tempo parado em cada setor, juntamente com quantos dias ele está parado a partir da sua última tramitação.
 
  - **Processos em tramitação por setor:** Gráfico de barras empilhadas que contabiliza quantos processos ainda estão em tramitação em cada setor da SAGEP.
 
  - **Tabela de processos críticos:** Uma tabela com o nº de protocolo, setor de origem, setor de destino e o tempo em que ele está parado. A criticidade é definida pelos processos que estão a mais de 2 dias sem receber uma resposta.
 
  - **Filtro setor traduzido:** Um filtro para mostrar apenas os dados do(s) setor(es) selecionado(s).
 
  - **Em tramitação:** Card que contabiliza quantos processos ainda estão em tramitação na SAGEP.
 
  - **Arquivados:** Card que contabiliza quantos processos não se encontram na SAGEP.
 
  - **Total:** Card que contabiliza quantos processos se econtram dentro caixa de processos da SAGEP.
 
  ## Como Usar

1. **Instalação:** Primeiro se certifique de instalar as seguintes aplicações:
  - Power BI Desktop: https://www.microsoft.com/pt-br/download/details.aspx?id=58494
  - Anaconda: https://docs.anaconda.com/free/anaconda/install/index.html
  - Visual Studio Code: https://code.visualstudio.com/docs/setup/windows
2. **Criando ambiente no Anaconda:**
  2.1 **Abrir o terminal ou Anaconda Prompt:** Abra o terminal ou Anaconda Prompt em seu sistema operacional.
  2.2 **Navegar até o diretório do ambiente virtual:** Use o comando 'cd' para navegar até o diretório onde o ambiente virtual está localizado. Por exemplo, se o ambiente virtual está em sua pasta "Downloads", você usaria o comando:
   'cd Downloads/Consulta-PAE'
  2.3 **Criano o ambiente virtual:** Uma vez no diretório correto, você pode criar o ambiente virtual usando o comando 'conda env create', seguido do nome do arquivo YAML. Supondo que o arquivo seja Consulta-PAE.yml, o comando seria:
   'conda env create -f Consulta-PAE.yml'
  2.4 Incie o ambiente virtual.
3. Inicie o arquivo Automacao_SAGEP_Busca_Processos_Judiciais.py, após ele finalizar sua operação os outros irão iniciar automaticamente, gerando as planilhas necessárias para o dashboard.
4. **Dados:** Certifique-se de que os dados estejam no formato correto e local adequado.
5. **Carregamento:** Abra o Power BI e carregue o arquivo `.pbix` deste repositório.
6. **Atualizando:** Após a primeira utilização atualize o dashboard clicando na opção "Atualizar".

## Contribuindo

Gostaria de contribuir? Fantástico! Aqui estão os passos:

1. **Fork** este repositório.
2. Crie uma nova **Branch** para suas modificações.
3. Faça suas alterações ou adições.
4. Faça um **Pull Request** para que possamos avaliar.

## Contato

Adriano Pinheiro - [EMAIL]
João Gabriel - jgteixeiraramos@gmail.com

   
