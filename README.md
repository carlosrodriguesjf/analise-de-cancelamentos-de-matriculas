
# ANÁLISE DE SOLICITAÇÔES DE CANCELAMENTO DE MATRÍCULA DA UFJF

## 👤 Autor e Contato
- **Nome**: Carlos Rodrigues
- **E-mail**: carlosrodriguesjf@gmail.com
- **LinkedIn**: https://www.linkedin.com/in/carlosrodriguesjf/
- **GitHub**: https://github.com/carlosrodriguesjf



## 📌 Descrição
O controle e a análise do cancelamento de matrículas são fundamentais para instituições de ensino, pois permitem identificar falhas no suporte acadêmico, financeiro e pedagógico oferecido aos estudantes. Com esses insights, a instituição pode desenvolver estratégias mais eficazes para retenção de alunos, aprimorar políticas institucionais e otimizar a gestão acadêmica, contribuindo para a redução da evasão e o fortalecimento do ensino superior.

Este projeto tem como objetivo identificar padrões e fatores que influenciam a saída dos alunos. Através da coleta, processamento e visualização dos dados, busca-se compreender os principais motivos da evasão, bem como principalmente, sua distribuição por campus, tipo de ingresso, curso e área de estudo, fornecendo informações essenciais para embasar a tomada de decisões institucionais.

Ao ingressar na instituição o estudante é alocado em grupo de cotas, conforme a seguir:

- Grupo A: Candidatos (as) autodeclarados (as) pretos (as), pardos(as) ou indígenas, com renda familiar bruta per capita igual ou inferior a um salário mínimo e que tenham cursado integralmente o ensino médio em escolas públicas;
- Grupo B: Candidatos(as) com renda familiar bruta per capita igual ou inferior a um salário mínimo que tenham cursado integralmente o ensino médio em escolas públicas;
- Grupo C: Ampla concorrência, independentemente da declaração de renda, de escola, de cor ou de origem racial;
- Grupo D: Candidatos(as) autodeclarados(as) pretos(as), pardos(as) ou indígenas que, independentemente da renda tenham cursado integralmente o ensino médio em escolas públicas;
- Grupo E: Candidatos (as) que independentemente da renda tenham cursado integralmente o ensino médio em escolas públicas;
- Grupo G: Candidatos(as) autodeclarados quilombolas, com renda familiar bruta per capita igual ou inferior a um salário mínimo e que tenham cursado o ensino médio integralmente em escolas públicas;
- Grupo H: Candidatos(as) com deficiência, que tenham renda familiar per capita igual ou inferior a um salário mínimo e que tenham cursado
integralmente o ensino médio em escolas públicas;
- Grupo I: Candidatos autodeclarados quilombolas, independentemente de renda, que tenham cursado integralmente o ensino médio em escolas
públicas;
- Grupo J: Candidatos com deficiência, independentemente da renda, que tenham cursado integralmente o ensino médio em escolas públicas;



## 🔍 Considerações Iniciais
- Usaremos uma base de base criada no chatGPT. Foram incluídos cursos verdadeiros de uma Universidade e motivos reais de cancelamentos apresentados por alunos.



## 🎯 Objetivos
**1. Identificar Padrões e Tendências na Evasão**
- Analisar a evolução dos cancelamentos ao longo do tempo.
- Verificar sazonalidade ou picos de cancelamento em determinados períodos.
- Comparar o número de cancelamentos entre diferentes anos de ingresso.

**2. Entender o Perfil dos Estudantes que Cancelam**
- Avaliar a relação entre idade e evasão. ------ok
- Analisar diferenças de cancelamento entre gêneros.------------ok
- Analisar se estudantes de ingressos mais recentes ou mais antigos têm maior propensão ao cancelamento ----------ok 
- Identificar quais grupos de cotas apresentam maiores taxas de desistência.

**3. Avaliar a Influência do Campus e do Curso**
- Comparar taxas de cancelamento entre diferentes campi.
- Verificar quais cursos e áreas de estudo têm maior evasão.
- Identificar se cursos de determinadas áreas têm padrões diferentes de cancelamento.

**4. Investigar os Principais Motivos do Cancelamento**
- Mapear as razões mais frequentes para o cancelamento.
- Identificar se certos perfis de estudantes têm motivos específicos para desistência.

**5. Relacionar o Tipo de Ingresso com a Evasão**
- Analisar se estudantes que ingressaram por diferentes modalidades (vestibular, ENEM, transferência, etc.) apresentam padrões distintos de cancelamento. -------ok
- Verificar se há diferenças entre alunos que ingressaram por ampla concorrência e por cotas.



## 📂 Estrutura do Projeto
```
📁 analise_cancelamento
│── 📂 dados                  # Conjunto de dados brutos e processados
│── 📂 testes                 # Jupyter Notebooks utilizado para testes de programação
│── 📂 scripts                # Scripts utilizados para automação, pré-processamento de dados e arquivo da análise
│── 📂 relatórios             # Relatórios e visualizações geradas
│── README.md                 # Documentação do projeto
│── requirements.txt          # Dependências do projeto


```

## 📊 Dados Utilizados
Os dados do arquivo base-cancelamentos-tratada.xlsx possuem as seguintes colunas:
- **Data protocolo**: Data em que a solicitação de cancelamento foi protocolada
- **Sexo**: Sexo dos solicitantes 
- **Data nascimento**: Data de nascimento dos solicitantes
- **Campus**: Campus onde os solicitantes estudavam
- **Motivo para cancelamento**: Motivo apresentado pelos os solicitantes
- **Curso**: Curso dos solicitantes
- **Área**: Área do curso dos solicitantes
- **Tipo de ingresso**: Forma em que os solicitantes foram aprovados na Universidade
- **Pontuação**: Pontuação tirada no processo de seleção
- **Ano Ingresso**: Ano de ingresso
- **Grupo de cotas**: Grupo de Cotas dos solicitantes




## 🛠️ Tecnologias e Ferramentas
- **Python**
- **Pandas**
- **Matplotlib**
- **Jupyter Notebook**



## 🚀 Como Executar o Projeto
1. Clone este repositório:
   ```bash
   git clone https://github.com/carlosrodriguesjf/analise-de-cancelamentos-de-matriculas-da-ufjf.git
   cd analise-de-cancelamentos-de-matriculas-da-ufjf\scripts
   ```
2. Crie um ambiente virtual e instale as dependências:
   ```bash
   python -m venv venv

   source venv/bin/activate  # No Linux
   \venv\Scripts\activate  # No Windows

   pip install -r requirements.txt
   ```
3. Execute os notebooks ou scripts:
   ```bash
   jupyter notebook
   ```
4. Para executar o tratamento da base:
   ```bash
   python scripts/tratamento-base.py
   ```
5. Para executar a análise de dados:
   ```bash
   python scripts/analise-de-dados.py



## 📈 Resultados e Insights
- **Distribuição de cancelamentos por sexo**: 
   - Mais estudantes do sexo feminino solicitaram o cancelamento (aproximadamente 53%). A diferença das solicitações dos gêneros é de 6,32%.

- **Distribuição de cancelamentos por ano de ingresso na instituição**: 
   - Podemos observar um aumento progressivo de acordo com o ano de ingresso, culminando no ano de 2023, onde aconteceu 308 pedidos. 
   - Um aumento de cerca de 33% em relação as pessoas que ingressaram no ano anterior. 
   - Em 2024 as solicitações diminuiram cerca de 34%

- **Distribuição de cancelamentos por idade**: 
   - Podemos concluir que os alunos que pediram mais cancelamentos tem a idade de 19 anos, seguido de 20 e 21

- **Distribuição de cancelamentos por tipo de ingresso**: 
   - Verificamos que ingressante pelo SISU possuem mais que o dobro de cancelamentos pdo que o segundo que é o PISW

- **Principais motivos de cancelamento**: [Descreva]
- **Distribuição por campus e curso**: [Descreva]
- **Correlação entre ingresso e evasão**: [Descreva]
- **Evolução ao longo dos anos**: [Descreva]



## 🔮 Objetivos Futuros
- **Expansão da base de dados**: Inclusão de novos dados para a verificação se os padrões ,0permanecem
- **Automatização de análises**: Elaborar um modelo de machine learning para prever tendências


