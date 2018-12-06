# desafio-python-dev

Criar um scrapper capaz de buscar os dados de todos os senadores ativos.

Este scrapper deve ser construido utilizando python 3 (ou superior) e beautifulSoup.

O código deve estar no formato de package seguindo os padrões de packages do pypi ( https://packaging.python.org/tutorials/packaging-projects/ )

A package deve ter os seguintes métodos

- obtemTodosSenadoresAtivos
  > Retorna lista de todos os senadores ( Exemplo de lista abaixo )
- obtemDetalhesDoSenador(id_senador)
  > Retorna dados mais detalhados de um senador em questão ( Exemplo de objeto abaixo ). 
  É importante que este método retorne o maior número de informações possíveis e dentro do formato do exemplo.
  
  Todas as proposicoes do parlamentares devem estar no objeto assim como todas as proposições relatadas.
  
  Os campos "chapas", "comissoes", "missoes" "biografia" devem ser preenchidos com o maior número de informações, clareza e organização possíveis.

Exemplo de lista de senadores ativos:

```
[
  {
    "nome":'Gladson Cameli',
    "partido": "PP",
    "uf": "AC",
    "periodo":"2015 - 2023",
    "telefones":"(61) 3303-1357 / 1367",
    "email": "gladson.cameli@senador.leg.br"
    "linkPagina":"https://www25.senado.leg.br/web/senadores/senador/-/perfil/4558",
    "id_senador":4558
  },
  ...
]
```

Exemplo de objeto de detalhes do Senador:

```
{

  "nomeCivil": "Gladson de Lima Cameli",
  "dataNascimento": "26/03/1978",
  "naturalidade": "Cruzeiro do Sul (AC)",
  "enderecoGabinete": "Senado Federal Anexo 2 Ala Teotônio Vilela Gabinete 14",
  "telefones": "(61) 3303-1357 / 1367",
  "email": "gladson.cameli@senador.leg.br",
  "sitePessoal": "URL_SITE_SENADOR",
  "enderecoEscritorioApoio": "AVENIDA TRAVESSA BOA VISTA, 111. ISAURA PARENTE, RIO BRANCO, AC.",
  "cep":69918306,
  "chapas": [],
  "comissoes": [],
  "missoes": [],
  "biografia":[],
  "proposicoes":["SF PEC 88/2015","SF PLS 330/2018", ... ],
  "materiaRelatadas": ["SF PDS 41/2016", "SF PDS 49/2016"]
}
```


Lista de Senadores em exercício:

https://www25.senado.leg.br/web/senadores/em-exercicio
