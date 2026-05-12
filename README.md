# Checkpoint 02 — Modelagem Linear Para Aprendizado de Máquina

**Tema:** Variáveis estatísticas e distribuição de frequências
**Turmas:** 1CCPJ | 1CCPK
**Formato:** Atividade em grupo | 1 hora | Entrega: notebook Python (.ipynb)

## Contexto

Antes de aplicar qualquer modelo preditivo, é necessário compreender a natureza dos dados com os quais se trabalha. Esta atividade parte desse princípio: o grupo deverá localizar uma base de dados real, identificar suas variáveis, classificá-las corretamente e construir tabelas de distribuição de frequências que façam sentido analítico — não apenas técnico.

A escolha da base de dados não é trivial. Ela exige julgamento, e é parte da avaliação.

## Instruções

### 1. Escolha da base de dados

O grupo deverá selecionar uma base de dados pública com as seguintes características obrigatórias:

- Conter ao menos uma variável qualitativa nominal
- Conter ao menos uma variável qualitativa ordinal
- Conter ao menos duas variáveis quantitativas — uma discreta e uma contínua
- Ter no mínimo 200 registros
- Não ser um dataset de tutorial — Titanic, Iris, mtcars, Boston Housing e similares não serão aceitos

Fontes sugeridas, mas não obrigatórias: Kaggle, UCI Machine Learning Repository, dados.gov.br, IBGE, INEP, Portal da Transparência, Our World in Data.

### 2. Justificativa da escolha

Na primeira célula de texto do notebook, o grupo deve redigir um texto com no mínimo 150 palavras explicando por que esta base foi escolhida, qual é o contexto real dos dados (quem os coletou, para quê e quando), por que ela é adequada para os objetivos desta atividade e quais limitações ou ressalvas o grupo identifica nos dados. Respostas genéricas ou que reproduzam a descrição original do dataset não serão aceitas.

### 3. Classificação das variáveis

O grupo deve apresentar uma tabela com todas as colunas do dataset, contendo:

| Coluna | Tipo | Subtipo | Justificativa |
|--------|------|---------|---------------|
| ...    | qualitativa / quantitativa | nominal / ordinal / discreta / contínua | ... |

A coluna de justificativa deve ser preenchida com argumentação própria. Classificações sem justificativa receberão pontuação zero neste critério.

### 4. Tabelas de distribuição de frequências

Para cada tipo de variável identificado, o grupo deve construir ao menos uma tabela de distribuição de frequências. Para variáveis qualitativas e quantitativas discretas: frequência absoluta, frequência relativa e frequência acumulada quando aplicável. Para variáveis quantitativas contínuas: distribuição por classes, com justificativa do número de classes escolhido, referenciando a regra utilizada (Sturges, Scott ou outra).

As tabelas devem ser construídas com código Python. O uso isolado de `.value_counts()` sem tratamento, formatação ou organização adequada não será considerado suficiente.

### 5. Análise interpretativa

Para cada tabela gerada, o grupo deve escrever ao menos dois parágrafos interpretando o que os dados mostram. Não se trata de descrever a tabela — trata-se de extrair significado dela no contexto real do dataset.

## Estrutura esperada do notebook

```
1. Identificação do grupo e do apresentador
2. Escolha e justificativa da base de dados
3. Carregamento e inspeção inicial dos dados
4. Classificação das variáveis (tabela completa com justificativas)
5. Tabelas de distribuição de frequências
   5.1 Variável qualitativa nominal
   5.2 Variável qualitativa ordinal
   5.3 Variável quantitativa discreta
   5.4 Variável quantitativa contínua
6. Interpretação analítica
7. Conclusão: o que a distribuição dos dados revela sobre o problema real?
```

## Critérios de avaliação

| Critério | Peso |
|----------|------|
| Adequação e originalidade da base de dados escolhida | 15% |
| Qualidade da justificativa da escolha | 15% |
| Correção e completude na classificação das variáveis | 20% |
| Construção técnica das tabelas de frequência | 25% |
| Qualidade da interpretação analítica | 20% |
| Apresentação oral — clareza, domínio e capacidade de justificar as escolhas | 5% |

Trabalhos que utilizarem bases não aceitas, apresentarem justificativas copiadas ou tabelas geradas sem código próprio serão zerados independentemente dos demais critérios. Grupos que não realizarem a apresentação não terão a entrega considerada.

## Entrega

Formato: arquivo `.ipynb` com todas as células executadas. O notebook deve ser autocontido — quem o abrir deve conseguir reproduzir todos os resultados. Os nomes de todos os integrantes e do apresentador devem constar na primeira célula. O arquivo deve ser anexado à tarefa no Teams até o encerramento da atividade.

## Observação final

Esta atividade não tem resposta certa. Tem resposta bem argumentada ou mal argumentada. O grupo que conseguir explicar por que fez cada escolha — da base de dados ao número de classes — está no caminho correto.
