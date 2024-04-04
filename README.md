# Extrator de Reviews da Steam

Este script Python permite extrair reviews de jogos da Steam, filtrando por idioma (português brasileiro) e tipo de review (positiva ou negativa), e salvar essas informações em um arquivo CSV.

## Funcionalidades
- Extrai reviews de um jogo específico da Steam utilizando o ID do jogo.
- Permite filtrar reviews por tipo (positivas ou negativas).
- Salva os dados coletados em um arquivo CSV para análise posterior.

## Dependências
Para executar este script, você precisará das seguintes bibliotecas Python:

- requests
- pandas

## Você pode instalar essas dependências usando o comando pip:
 
    pip install requests pandas

## Como Usar
Configuração Inicial: No início do script, configure os seguintes parâmetros:

- app_id: O ID do aplicativo/jogo na Steam.
- nome_do_jogo: O nome do jogo que você está interessado.
- num_per_page: Número de reviews por página (até um máximo de 100).
- tipo: Tipo de review ("positive" para reviews positivas, "negative" para reviews negativas).

## Execução do Script: 
Execute o script para iniciar a coleta de dados. As reviews serão coletadas e salvas em um arquivo CSV no formato jogo_APPID_steam_TIPO_ptBR.csv, onde APPID é o ID do aplicativo e TIPO é o tipo de review.

## Exemplo de Uso
Para extrair reviews positivas do jogo "Chroma Squad" (ID 251130), configure o script da seguinte maneira:

    app_id = "251130"
    nome_do_jogo = "Chroma Squad"
    num_per_page = 100
    tipo = "positive"

Em seguida, execute o script. O arquivo CSV gerado conterá as reviews positivas em português brasileiro.

## Limitações
Este script é específico para a Steam e foi projetado para funcionar com o idioma português brasileiro. Alterações na API da Steam podem requerer ajustes no código.

## Licença
[MIT](https://mit-license.org/)
