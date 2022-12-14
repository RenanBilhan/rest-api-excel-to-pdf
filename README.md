# rest-api-excel-to-pdf

Objetivo: Construir uma REST API que receba um XMLX, trate os dados e, a partir desses dados, seja capaz de emitir certificados em PDF com as informações coletadas do XMLX. A API cria certificados de horas de acordo com os dados listados no excel (nome, carga horária e nome do curso)

Por que uma API? Optei por utilizar o modelo de API puramente por interesse em estudar e praticar a criação de APIs REST.

Integração com banco de dados? Sim, integração feita através do JPA Hibernate, que facilita a interação entre a API e o banco de dados.

Método utilizado para recebimento do arquivo XML? Foi utilizado o FrameWork APACHE POI, possibilitando o recebimento e trabalho com arquivos XMLX. Através do método Create, a API recebe uma tabela XMLX e gera um modelo de certificado, que é adicionado a uma lista de certificados. O método Create retorna essa lista.

Método utilizado para criação dos PDFs? foi utilizado o editor JasperSoft, que além de disponibilizar alguns temas pré-prontos, possibilita criação e personalização de temas próprios, podendo gerar um certificado com logomarcas, etc. O método generatePdf recebe a lista de certificados criada anteriormente e acessa cada um dos certificados da lista, gerando um documento PDF para cada.

As funcionalidades foram testadas (de forma simples) com o programa PostMan.

Obrigado pelo interesse!!

