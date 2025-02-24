Modelar e projetar um sistema de banco de dados envolve definir a estrutura, os componentes e as regras de funcionamento do banco de dados para garantir que ele atenda aos requisitos da aplicação de forma eficiente e organizada.

************** 1. Modelagem de Banco de Dados ************
A modelagem é a fase conceitual onde se define a estrutura do banco de dados sem se preocupar com detalhes específicos da implementação. Ela inclui:

Modelo Conceitual: Representação abstrata dos dados, geralmente usando diagramas entidade-relacionamento (DER), onde se identificam entidades, atributos e relacionamentos.

Modelo Lógico: Conversão do modelo conceitual para um modelo que pode ser implementado em um banco de dados relacional (como tabelas, chaves primárias e estrangeiras).

Modelo Físico: Definição de detalhes técnicos, como tipos de dados, índices e normalização para otimizar a eficiência do banco.


********* 2. Projeto de Banco de Dados ***********
O projeto é a fase em que as definições feitas na modelagem são implementadas. Ele envolve:

Escolha do SGBD (Sistema Gerenciador de Banco de Dados) adequado (MySQL, PostgreSQL, SQL Server, etc.).
Criação das tabelas e relacionamentos de acordo com o modelo lógico.
Definição de restrições de integridade (chaves primárias, estrangeiras, unicidade, etc.).
Otimização de desempenho, como indexação e controle de concorrência.
Segurança e controle de acesso, garantindo que os dados sejam protegidos contra acessos não autorizados.

Modelagem = Planejamento e estruturação dos dados (o quê será armazenado e como se relacionam).
Projeto = Implementação técnica da modelagem em um SGBD (como os dados serão armazenados e acessados).


************ Sistema de gerenciamento de obra *****************   ||| Obra com proprietário--> engenheiro responsável-->pedreiros |||

Proprietário--> CPF, NOME, ENDEREÇO --> minimo 1 obra, máximo N

Engenheiro responsável--> CPF\CNPJ, NOME, ENDEREÇO, CREA ---> minimo 0,máximo N

Pedreiro --> CPF, NOME, ENDEREÇO  --> Minimo 0, máximo N



Exericio modelagem conceitual: 
1) Identificar entidades
2) identiticar atributos --> identificador
3) Identificar relacionamentos -->  Qual entidade se relaciona com qual
4) Mapear Cardinalidade







************* BANCO DE DADOS(SISTEMA DE VENDAS) ***********
Vendedor -- > CPF, NOME, --> Cardinalidade\ cliente --> (1,n)
Cliente --> CPF, NOME, ---> Cardinalidade\vendedor -->(1,n)
PRODUTO --> TIPO, MODELO, PRATELEIRA  --> Cardinalidade\vendedor --> (n,n) .._ Cardinalidade\cliente --> (n,n)



