# [Front]

## Introdução
MVP da Sprint 3 do curso de pós gradução em Engenharia de Software da PUC.
Trata-se de um Projeto (Obras de Arte) que a partir das opções do usuário na interface, seleciona APIs, com serviços específicos a serem consumidos, com o objetivo final de disponibilizar um link de uma imagem para uma dada Obra e Artista.

## Utilização do Aplicativo:
        
Este Projeto (Obras de Arte) tem por objetivo realizar o cadastro de obras de arte, sejam pinturas, esculturas ou outras. Este cadastro armazena o nome da obra, o nome do artista, o estilo de época da obra (Renascimento, Barroco, Neoclassicismo, dentre outros), além do tipo, que informa se é uma pintura, uma escultura ou outro tipo. Adicionalmente, cadastra-se também um link que direciona para um ambiente que traz informações adicionais à obra. Os campos: Obra, Artista, Estilo, Tipo e Link são utilizados para realizar o cadastro das obras, uma vez acionando o botão “Adicionar”. Os campos: Obra, Artista, Estilo e Tipo são campos obrigatórios (RN1). É permitido que o cadastro aconteça sem um link relacionado à obra. Não são permitidos cadastros de uma obra de mesmo nome e mesmo artista (RN2). Porém, caso haja uma obra de mesmo nome, mas para artistas diferentes, é permitida esta inserção.

O usuário pode optar por buscar um link de imagem para a obra, deixando o campo Link vazio, e respondendo ao questionamento do sistema de forma apropriada. Caso opte pela busca de um link de imagem, o sistema fará, primeiramente e automaticamente, através de uma API, a tradução do nome da obra de português para inglês, e realizará, também de forma automática, utilizando-se de uma segunda API, a busca pelo nome da obra (agora com o nome traduzido para o inglês) em um museu, e inserirá de volta na base, ou o link encontrado ou a informação de que, ou a obra não existe na base do museu consultado, ou o artista não existe na base do museu consultado. Todas as demais informações inicialmente inseridas nos demais campos serão mantidas como inseridas pelo usuário, inclusive o nome da obra em português, como inicialmente fornecida pelo usuário.

### OBS:

1 - RN::Regra de Negócio.

2 - O primeiro parágrafo acima trata da parte entregue na Sprint 1 (que foi reaproveitada), com algumas melhorias. Por exemplo, a otimização da RN2 colocando a consulta ao banco antes das chamadas às APIs, melhorando o tempo de retorno ao usuário quanto à realização da crítica.

3 - O segundo parágrafo acima, trata da parte implementada para esta Sprint 3 (API_B1 e API_B2).

## Arquitetura
Arquitetura do Projeto Obras de Arte com destaque para o FrontEnd, que seleciona a API a ser utilizada a medida das opções do usuário.

![Front](https://github.com/Moriblo/front/blob/main/Front.png)

## Estrutura do Código e Chamadas
Estrutura dos códigos de cada API e chamadas.

![COMP_A](https://github.com/Moriblo/front/blob/main/COMP_A.png)

## Projeto
Detalhamento dos requisitos (REQ) do MVP e demais issues tratados [https://github.com/users/Moriblo/projects/2/views/5]
