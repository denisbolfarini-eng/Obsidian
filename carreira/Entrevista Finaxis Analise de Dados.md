
### **1. Análise descritiva**

Como o próprio nome diz, a análise descritiva é um dos tipos de análise de dados baseado em fatos. Isso significa que, na prática, este tipo de avaliação de dados é feita a partir de resultados obtidos. São exemplos de análise de dados descritiva: 

- relatórios; 
- segmentação e [controle de clientes](https://www.zendesk.com.br/blog/controle-de-clientes/);
- análises de negócio; 
- aplicação de [métricas](https://www.zendesk.com.br/blog/metricas-vendas/); 
- avaliação de resultados. 

Um dos principais usos para a análise descritiva é orientar a construção de estratégias.

### **2. Análise preditiva**

O mais popular dos tipos de análise de dados é justamente o modelo preditivo. Como o nome diz, sua essência está na **previsão** de cenários futuros com base na análise de padrões revelados pela base de dados. 

É importante saber que, em uma análise preditiva, não é possível prever o que vai acontecer, mas sim, o que deve acontecer SE determinadas condições se cumprirem.

Quer ver um exemplo de análise de dados preditiva? 

Suponhamos que sua empresa esteja apreensiva quanto à possível entrada de um concorrente no mercado. A análise preditiva não será capaz de te dizer se o concorrente iniciará ou não suas atividades em breve. 

Em contrapartida, te ajudará a enxergar o que poderá acontecer SE o concorrente, de fato, entrar no mercado, tomando como base situações anteriores com contextos semelhantes. 

Podemos dizer, assim, que o objetivo da análise preditiva é determinar uma tendência, correlação, causa ou probabilidade.

### **3. Análise prescritiva**

A análise prescritiva é o próximo passo após os resultados da avaliação preditiva. Isso porque uma prescrição é uma recomendação a algo potencialmente previsto. 

Sendo assim, a melhor forma de obter uma análise prescritiva é fazendo projeções (predições) e, então, direcionando esforços para obter o melhor resultado a partir das possibilidades. 

Por ser uma análise de dados constantemente mutável (já que está sempre condicionada a previsões e predições), os modelos analíticos prescritivos são comumente apoiados por tecnologias como [inteligência artificial](https://www.zendesk.com.br/blog/inteligencia-artifical-atendimento-cliente/), [_machine learning_](https://www.zendesk.com.br/blog/machine-learning/) e algoritmos. 

As ferramentas ajudam a fazer sugestões com base em padrões diferenciados e percepções de objetivos organizacionais, limitações e fatores de influência.

### **4. Análise diagnóstica**

Aqui está outro tipo de análise de dados concentrada em algo que já aconteceu (assim como a análise descritiva). 

A análise diagnóstica, diferentemente da descritiva, tem, como objetivo, encontrar relações de causa e efeito para compreender um acontecimento. 

É claro que estabelecer este tipo de relação baseado em um acontecimento passado não é tarefa fácil. Por isso mesmo, o processo é baseado em **probabilidades**. 

Conhecer os principais tipos de análise de dados pode ajudar a sua empresa a dominar as informações-chave do negócio na palma da mão. 

Lembre-se de que é possível automatizar tarefas importantes da análise de dados (como a consolidação de relatórios e a criação de gráficos) com a ajuda das melhores ferramentas e tecnologias, como é o caso da inteligência artificial (IA).

Um analista de dados precisa dominar ==estatísticas descritivas (medidas de centralidade e dispersão), estatísticas inferenciais (testes de hipóteses, distribuições), probabilidade e, para funções mais avançadas, métodos de aprendizado de máquina e modelos preditivos==. Este conhecimento permite que o analista interprete dados com precisão, extraia insights valiosos, crie modelos para prever resultados e tome decisões informadas e confiáveis. 

Conceitos essenciais de estatística:

- **Estatística Descritiva:**
    
    - **Medidas de Centralidade:** Média, mediana e moda para entender o valor típico de um conjunto de dados. 
    - **Medidas de Dispersão:** Desvio padrão, variância e amplitude para entender a variabilidade dos dados. 
    - **Tipos de variáveis:** Compreender as diferentes categorias de dados (qualitativos e quantitativos) é fundamental para a análise correta. 
    
- **Estatística Inferencial:**
    
    - **Probabilidade:** Fundamental para entender a incerteza nos dados e prever a ocorrência de eventos. 
    - **Testes de Hipóteses:** Essencial para comparar grupos e determinar a significância estatística de um resultado, como em testes A/B para analisar a taxa de conversão. 
    - **Distribuições:** Conhecer as principais distribuições estatísticas (normal, binomial, etc.) ajuda a modelar e interpretar os dados de forma mais precisa. 
    

Aplicação prática da estatística para o analista:

- **Extração de Insights:** 
    
    A estatística é o que transforma dados brutos em conhecimento, permitindo que o analista descubra padrões e tendências não óbvias. 
    
- **Tomada de Decisão:** 
    
    Permite basear recomendações e planos de ação em evidências concretas, evitando decisões baseadas em "achismos". 
    
- **Modelagem e Previsão:** 
    
    Em funções mais avançadas, o conhecimento estatístico é a base para construir e validar modelos preditivos, como regressão, que preveem resultados futuros com base em dados históricos. 
    
- **Comunicação de Resultados:** 
    
    O analista precisa comunicar os achados de forma clara e confiante, explicando por que os insights são importantes e quais ações podem ser tomadas. 
    

Em suma, a estatística é o alicerce do analista de dados, fornecendo as ferramentas e o raciocínio crítico para trabalhar com dados de forma eficiente, confiável e a gerar valor para as organizações

A análise exploratória de dados (AED) em SQL ==é o processo de usar consultas para examinar e resumir as características principais de um conjunto de dados, identificando tendências, padrões e erros como valores faltantes ou outliers==. O SQL, através de comandos como `SELECT`, `WHERE`, `GROUP BY` e funções estatísticas, permite extrair, filtrar e agregar dados para entender melhor seu conteúdo e preparar os dados para análise ou modelagem. 

Passos da Análise Exploratória com SQL

1. **Extração e Filtragem de Dados:**
    
    - Use `SELECT` para escolher as colunas desejadas. 
    - Aplique `WHERE` para filtrar linhas que atendem a condições específicas, focando em um subconjunto de dados. 
    - Utilize `JOIN` para combinar dados de várias tabelas, enriquecendo o conjunto de dados para análise. 
    
2. **Resumo Estatístico:**
    
    - Use `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()` para calcular estatísticas básicas, como contagem, soma, média, valor mínimo e máximo de colunas. 
    - Utilize `GROUP BY` para agregar linhas com valores idênticos em uma coluna, permitindo a criação de tabelas de frequência ou resumos por categoria. 
    - Aplique `HAVING` para filtrar os grupos resultantes de uma agregação. 
    
3. **Identificação de Padrões e Anomalias:**
    
    - Analise a distribuição dos dados usando consultas que retornam a frequência de cada valor ou a contagem de valores únicos com `COUNT(DISTINCT coluna)`. 
    - Identifique valores discrepantes (outliers) ou dados faltantes (`NULL`) que precisam de tratamento. 
    - Use funções como `UPPER()`, `LOWER()` e `TRIM()` para normalizar dados de texto e garantir a consistência. 
    
4. **Visualização (Externa ao SQL, mas informada por ele):**
    
    - Embora o SQL não crie gráficos diretamente, os resultados das consultas podem ser exportados para ferramentas de visualização.
    - Use esses resultados para criar histogramas, gráficos de barras e boxplots, que são essenciais para entender a distribuição dos dados e identificar outliers. 
    

Por que usar SQL para AED?

- **Eficiência:** 
    
    O SQL é otimizado para manipular grandes volumes de dados diretamente nos bancos de dados relacionais. 
    
- **Poder:** 
    
    Permite consultas complexas para extrair e manipular dados, o que é crucial para a análise de grandes conjuntos. 
    
- **Base:** 
    
    O SQL fornece os insights iniciais necessários antes de aplicar modelos mais complexos de Machine Learning, ajudando a preparar os dados de forma eficaz.


Descrição vaga

Olá Pessoal!!!  
Sextouu hein?! E para fechar com "chave de Ouro", temos vagas!!! 😁  
  
Analista de Inteligência de Dados(Desenvolvedor) Júnior - CLT  
São Paulo - Híbrido  
Seg a Sex 09:00 12:00 13:00 18:00  
  
Responsabilidades:  
Criar, corrigir e revisar soluções em Cloud, aplicando scripts confiáveis, reutilizáveis e performáticos;  
Criar ou atualizar as documentações relacionadas, fazendo uso de boas práticas e padrões de desenvolvimento;  
Atender às necessidades de visualização de dados, utilizando diversas ferramentas e linguagens, alinhadas ao que há de mais atual;  
Documentar os processos de atualização e as soluções criadas.  
  
Requisitos:  
Superior em tecnologia (mínimo cursando);  
Python;  
Ferramentas de banco de dados, como Microsoft SQL, Oracle ou PostgreSQL;  
Experiências desejáveis:  
HTML;  
CSS;  
JavaScript;  
Node.js;  
Angular;  
Arquitetura On-Premise (Airflow, Docker, Linux);  
Arquitetura Azure (Datafactory, Datalake, Databricks, Web App Service).  
  
Faz sentido para você? É só clicar no link abaixo e concluir sua candidatura.  
Não faz sentido? Compartilha com alguém que esteja buscando 😉