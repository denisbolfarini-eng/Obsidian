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
- Fluxos : Quando existe um alteração é disparado a alteração







