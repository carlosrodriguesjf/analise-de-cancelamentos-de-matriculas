
# ANÁLISE DOS DADOS DE CANCELAMENTO DE MATRÍCULA DE UMA UNIVERSIDADE

## 👤 Autor e Contato
- **Nome**: Carlos Rodrigues
- **E-mail**: carlosrodriguesjf@gmail.com
- **LinkedIn**: https://www.linkedin.com/in/carlosrodriguesjf/
- **GitHub**: https://github.com/carlosrodriguesjf



## 📌 Descrição
O controle e a análise do cancelamento de matrículas são fundamentais para instituições de ensino, pois permitem identificar falhas no suporte acadêmico, financeiro e pedagógico oferecido aos estudantes. Com esses insights, a instituição pode desenvolver estratégias mais eficazes para retenção de alunos, aprimorar políticas institucionais e otimizar a gestão acadêmica, contribuindo para a redução da evasão e o fortalecimento do ensino superior.

Este projeto tem como objetivo identificar alguns padrões e fatores que influenciam a saída dos alunos. Através da coleta, processamento e visualização dos dados, busca-se compreender os principais motivos da evasão, bem como principalmente, sua distribuição por campus, tipo de ingresso, curso e área de estudo, fornecendo informações essenciais para embasar a tomada de decisões institucionais.

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

**1. Entender o Perfil dos Estudantes que Cancelam**
- Avaliar a relação entre sexo e evasão.
- Avaliar a relação entre idade e evasão.
- Analisar se estudantes de ingressos mais recentes ou mais antigos têm maior propensão ao cancelamento
- Identificar quais grupos de cotas apresentam maiores taxas de desistência.


**2. Identificar Padrões e Tendências na Evasão**
- Analisar a evolução dos cancelamentos ao longo do tempo.


**3. Avaliar a Influência do Campus e do Curso**
- Comparar taxas de cancelamento entre diferentes campi.
- Verificar quais cursos e áreas de estudo têm maior evasão.
- Identificar se cursos de determinadas áreas têm padrões diferentes de cancelamento.


**4. Investigar os Principais Motivos do Cancelamento**
- Mapear as razões mais frequentes para o cancelamento.



**5. Relacionar o Tipo de Ingresso com a Evasão**
- Analisar se estudantes que ingressaram por diferentes modalidades (vestibular, ENEM, transferência, etc.) apresentam padrões distintos de cancelamento. 
- Verificar se há diferenças entre alunos que ingressaram por ampla concorrência e por cotas.



## 📂 Estrutura do Projeto
```
📁 analise_cancelamento
│── 📂 dados                 # Conjunto de dados brutos e processados
│── 📂 testes                # Jupyter Notebooks utilizado para testes de programação
│── 📂 scripts               # Scripts utilizados para automação, pré-processamento de dados e arquivo da análise
│── 📂 relatórios            # Pasta contendo um relatório com todos os códigos e visualizações
│── README.md                # Documentação do projeto
│── requirements.txt         # Dependências do projeto


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
4. Para executar a análise de dados:
   ```bash
   python scripts/analise-de-dados.py
   ```




## 📈 Resultados e Insights
- **Distribuição de cancelamentos por sexo**: 
   - Mais estudantes do sexo feminino (cerca de 53%)  solicitaram o cancelamento das sua matrícula. Ligeiramente 6% a mais do que o sexo masculino.


- **Distribuição de cancelamentos por idade**: 
   - Podemos concluir que os alunos que pediram mais cancelamentos são os alunos mais novos - 18 anos, seguidos os de 19 anos


- **Distribuição de cancelamentos por ano de ingresso na instituição**: 
   - Podemos observar um aumento progressivo de acordo com o ano de ingresso, culminando no ano de 2023, onde aconteceu 442 pedidos. 
   - Um aumento de cerca de 37% em relação as pessoas que ingressaram no ano anterior. 
   - Já no ano seguinte, em 2024, as solicitações diminuiram cerca de 62%


- **Distribuição de cancelamentos por grupo de cotas**: 
   -  Verificamos que o grupo que apresentou expressivamente mais solicitações de cancelamento foi o Grupo C - Ampla concorrência, independentemente da declaração de renda, de escola, 
 de cor ou de origem racial seguido do Grupo E - Candidatos (as) que independentemente da renda tenham cursado integralmente o ensino médio em escolas públicas e Grupo A - 
 Candidatos (as) autodeclarados (as) pretos (as), pardos(as) ou indígenas, com renda familiar bruta per capita igual ou inferior a um salário mínimo e que tenham cursado integralmente o ensino médio em escolas públicas


- **Distribuição de cancelamentos ao longo do tempo**: 
  - A quantidade de cancelamentos foi maior em 2023, indicando um possível pico nesse ano. 2021 e 2022 apresentaram números próximos, sugerindo estabilidade. 2024 mostra uma leve redução em relação a 2023, mas ainda em patamares elevados. 2020 teve o menor número, possivelmente influenciado por fatores como a pandemia. 


- **Distribuição de cancelamentos por campi**: 
  - O campus de Juiz de Fora apresenta o maior número de cancelamentos (824), significativamente superior aos demais, indicando possíveis desafios específicos na retenção de alunos. Salvador (270), Rio de Janeiro (236) e São Paulo (220) possuem volumes semelhantes, sugerindo uma distribuição mais equilibrada de cancelamentos nesses locais. A disparidade entre Juiz de Fora e os outros campi pode indicar fatores regionais, institucionais, específicos dos cursos oferecidos ou talvez por ter mais alunos do que os outros campi.
  - A área de estudos dos alunos que mais solicitam cancelamento é àrea de Humanas sendo que nessa área os alunos que mais cancelam são dos cursos BACHARELADO INTERDISCIPLINAR EM CIÊNCIAS HUMANAS, DIREITO e CIÊNCIAS ECONÔMICAS
  - Na área de Exatas, segundo colocado no ranking de mais cancelamentos os alunos que mais cancelam são dos cursos de CIÊNCIAS EXATAS, QUÍMICA e ENGENHARIA CIVIL	
  - Finalmente, na área de saúde, os alunos que mais cancelam são dos cursos de MEDICINA, NUTRIÇÃO, FARMÁCIA


- **Distribuição de cancelamentos por motivo**: 
  - Independente do campus ou dos cursos, os motivos predominantes são Dificuldades financeiras e Falta de identificação ou interesse pelo curso


- **Distribuição de cancelamentos por tipo de ingresso**: 
   - Os cancelamentos são dominados por alunos que ingressaram pelo SISU (915), seguido pelo PAS (405), indicando que esses processos seletivos representam a maior parte das desistências. Vestibular (139) tem um volume menor, mas ainda relevante. As demais formas de ingresso possuem números significativamente mais baixos, com destaque para Transferência (8), Mudança de Curso (1) e Nova Modalidade/Habilitação (18), sugerindo que alunos que entram por essas vias tendem a permanecer mais na instituição. O alto número de cancelamentos via SISU e PAS pode indicar desafios na adaptação desses alunos ao curso ou à universidade.




## 🔮 Objetivos Futuros
- **Expansão da base de dados**: Inclusão de novos dados para a verificação se os padrões permanecem
- **Automatização de análises**: Elaborar um modelo de machine learning para prever tendências


