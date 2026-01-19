- Coletamos dados, Preparamos os Dados, Exploramos, Experimentação e Predição
- Os Engenheiros de Dados são responsáveis pela primeiro parte processo.
- Os dados corretos, na forma correta, para as pessoas corretas, da forma mais eficiente possível
- Dar entrada nos dados de diferentes fontes; Otimizar bancos de dados para análise; Remover dados corrompidos; Desenvolver, construir, testar e manter arquiteturas de dados
- Big Data (Volume, Variedade, Velocidade, Veracidade e Valor)

# Engenheiro x Cientista
- Eng se concentram na primeira parte do fluxo de trabalho.
- Cien atuam no restante do fluxo do trabalho
- Eng estabelecem a base
- Eng -> Dar entrada nos dados e armazená-los | Configurar banco de dados | Criar Pipelines de dados | Sólidas habilidades em software 
- Cien > Explorar dados | Acessar banco de dados | Usam pipelines | Fortes habilidades analíticas 

# Pipeline de dados
- Dar entrada
- Processar
- Armazenar
- Necessidade de pipelines
- Automatizar o fluxo de uma estação para outra
- Disponibilizar dados atualizados, precisos e relevantes 

- Pipelines são os caminhos dos dados

- Automatizam {
	  - Extração
	  - Transformação
	  - Combinação
	  - Validação
	  - Carregamento
- }

- Reduzem {
	- Intervenção humana
	- Erros
	- Tempo necessário para movimentação dos dados
  }

- ETL - Extração, Transformação e Carregamento

# Estrutura de Dados

-  Fáceis de pesquisar e organizar
- Modelo uniforme, com linhas e colunas
- Tipos definidos
- Podem ser agrupados para formar relações
- Armazenados em bancos de dados relacionais
- São criados e consultados usando SQL

Dados semiestruturados
- Relativamente fáceis de pesquisar e organizar
- Modelo uniforme, implementação menos rígida: observações diferentes têm tamanhos diferentes
- Tipos diferentes
- Podem ser agrupados, mas isso requer mais trabalho
- NoSQL: JSON, XML, YAML

Não estruturados:
- Não seguem um modelo, não cabem em linhas e colunas.
- Difíceis de pesquisa e organizar.
- Geralmente texto, som, imagens ou vídeos.
- Normalmente em data lakes, podendo aparecer em data warehouses ou bancos de dados

# Banco de dados SQL

- Sistema de Gerenciamento de Bancos de Dados Relacionais (RDBMS)
- Permitir acessar muitos registros de uma só vez e os agrupe, filtre ou agregue
- Parecido com inglês
- Eng criar tabelas
- Cient consultam

# Data warehouses e data lakes
- Datalake:
	- Armazena todos os dados brutos
	- Pode ser de petabytes (1 milhão de GBs)
	- Armazena todas as estrutura de dados
	- Bom custo-benefício
	- Difícil de analisar
	- Requer um catálogo de dados
	- Usado por cientistas de dados
	- Big data, análise em tempo real
- Data warehouse:
	- Dados específicos para uso específico
	- Relativamente pequeno
	- Armazena principalmente dados estruturados
	- Mais caro para atualizar
	- Otimizado para análise de dados
	- Também usado por analistas de dados e analistas de negócios
	- Consultas conforme a necessidade, somente leitura
- Catalogo de dados para datalakes:
	- Fonte de verdade que compensa a falta de estrutura
	- Qual é a fonte desses dados?
	- Onde esses dados são usados?
	- Quem é o proprietário dos dados?
	- Com que frequência esses dados são atualizados?
	- Boas práticas de governança de dados
	- Garante reprodutividade
	- Sem catálogo --> data swamp (pântano de dados)
	- Boas práticas:
		- Confiabilidade
		- Autonomia
		- Escalabilidade
		- Velocidade


## Banco de dados x data warehouse

- Banco de dados:
	- Dados organizados e armazenados em computador (termo geral)
- Data warehouse:
	- É um tipo de banco de dados


# Movimentação e processamento de dados

## Processamento de dados
- Conversão de dados brutos em informações proveitosas
- Remover dados indesejados
- Otimizar custos
- Conversão de dados
- Organizar dados
- Seguir esquema/estrutura
- Aumentar produtividade
### Como os engenheiros de dados processam os dados
- Tarefas de manipulação, limpeza e organização de dados -> Automatizadas, Sempre precisaram ser feitas
- Armazenam dados em um banco de dados estruturado de forma sensata
- Criam exibições com base nas tabelas do banco de dados
- Otimizam o desempenho

## Agendamento de dados 
- Aplicada a qualquer tarefa do processamento de dados 
- Coesão
- Organiza o funcionamento do conjunto-
- Execução em uma ordem específica
### Agendamento manual, por horário e por sensor
 - Manual
 - Automático em horário específico
 - Sempre é necessário um sensor
### Lotes e fluxos
- Agrupam em lotes, mais barato
- Fluxos : Quando existe um alteração é disparado a atualização

Ferramentas para agendamento = Apache Airflow e Luigi

## Computação paralela
- Base das ferramentas modernas de processamento de dados
- Necessária:
	- Principalmente por causa de memória 
	- Também pela capacidade de processamento
- Como Funciona:
	- Divisão das tarefas em várias subtarefas menores
	- Distribuição dessas subtarefas em vários computadores
### Benefícios e riscos da computação paralela
- Funcionários = unidades de processamento
- Capacidade de processamento extra
- Menos quantidade de memória
- Movimentação de dados acarreta custo
- Maior tempo de comunicação
## Computação em nuvem
- Alugados
- Não precisam de espaço
- Usam apenas os recursos necessários
- Quando forem necessários
- Quanto mais próximos do usuário, melhor
- Confiabilidade do banco de dados: replicação de dados
- Risco com dados confidenciais

AWS -> AWS S3 -> EC2 -> RDS
Azure -> Blob -> Azure Virtual Machines -> Azure SQL Database
G Cloud -> Cloud Storage -> Google Compute Engine -> Google Cloud SQL

Multinuvem 

# Junção de Dados no SQL

## Os prós e contras da INNER JOIN

- **Chave** é uma coluna única ou um grupo de colunas que identifica exclusivamente os registros em uma tabela.
-  **INNER JOIN**  procura registros em ambas as tabelas que correspondam a um determinado campo.
- Observação: Você deve usar o formato table.column_name ao selecionar colunas que existem em ambas as tabelas para evitar erro de SQL
- USING(nome_coluna) = quando o nome das colunas são idênticos

Sintaxe:

`SELECT`
  `f.id AS funcionario_id,      -- Pega o 'id' da tabela Funcionarios e renomeia`
  `f.nome AS nome_funcionario,    -- Pega o 'nome' da tabela Funcionarios e renomeia`
  `d.nome AS nome_departamento  -- Pega o 'nome' da tabela Departamentos e renomeia`
`FROM`
  `Funcionarios AS f`
`INNER JOIN`
  `Departamentos AS d ON f.departamento_id = d.id;`

`-- Exemplo hipotético com USING`
`SELECT *`
`FROM Funcionarios`
`INNER JOIN Departamentos USING(departamento_id);`

## Definições de relações

- 1 para muitos:
	- Uma única entidade pode se relacionar com muitas entidades
- 1 para 1:
	- Relação direta e única entre duas entidades em tabelas diferentes
- Muitos para muitos:
	- Muitas entidades podem se relacionar com muitas entidades em outra tabela

## Junções múltiplas


##  Junções externas, junções cruzadas e autojunções

- Left e Right JOIN junta todos os valores, até os não existentes

## FULL JOINs
 - Combinam um Right Join com um Left Join, ou seja retornam todos os valores

### Cross Join


# Teoria dos conjuntos em SQL

- Union -> Retorna todos os registros sem repetir os duplicados
- Union All -> Retorna todos os registros, até os duplicados
- Sintaxe
		![[Pasted image 20251004103123.png]]
- Os registros precisam ser parecidos

- Intersect = apenas registros em ambas as tabelas
![[Pasted image 20251004105908.png]]



Normalização de dados:

- Normalização é um processo para organizar dados em um banco de dados.
- Existem diferentes níveis chamados "formas normais" (normal forms).
- As três primeiras formas ajudam a evitar problemas como dados duplicados, dificuldades na inserção ou exclusão de informações.
- Cada nível tem regras específicas para garantir que os dados fiquem bem organizados e consistentes.

Niveis:

1FN: 
- Atomicidade: cada célula tem que ter apenas um valor
2FN: 
- Dependência Parcial: A tabela deve estar em 1FN e todos os atributos que não são chave devem depender da chave primária inteira
3FN:
- Dependência Transitiva: A tabela deve estar em 2FN e não pode haver dependência entre colunas que não são chaves 


Database views:

- Tabelas virtuais que não fazem parte do sistema fisico
- 








