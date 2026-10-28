# Análise de Dados para Redução do Turnover

Projeto de análise de dados aplicado à área de Recursos Humanos, com o objetivo de identificar fatores associados à rotatividade de funcionários (*turnover*) e propor ações para aumentar a retenção de talentos.

## Sobre o projeto

O setor de Recursos Humanos de uma empresa fictícia do ramo de tecnologia identificou a necessidade de compreender os fatores associados ao desligamento de colaboradores.

A partir dessa necessidade, foi realizada uma análise de dados para investigar o perfil dos funcionários, identificar grupos com maiores taxas de desligamento e avaliar quais características apresentavam maior associação com o turnover.

A principal pergunta de negócio foi:

**Quais políticas e fatores organizacionais poderiam ser revistos para reduzir o turnover e aumentar a retenção de colaboradores?**

## Objetivos

- Analisar o comportamento do turnover na empresa.
- Identificar grupos de funcionários com maiores taxas de desligamento.
- Investigar a relação entre características profissionais e rotatividade.
- Avaliar a relevância das variáveis por meio de técnicas estatísticas.
- Propor ações para apoiar a tomada de decisão do RH.
- Definir indicadores para acompanhar a evolução do turnover após a implementação das melhorias.

## Ferramentas utilizadas

- **Excel:** exploração inicial dos dados, organização de informações, tabelas e análises complementares.
- **Python:** análise exploratória de dados (AED), estatística descritiva, visualizações e aplicação de técnicas estatísticas.
- **Power BI:** construção de dashboards para visualização dos indicadores e acompanhamento do turnover.

## Metodologia

O projeto utiliza como referência a metodologia CRISP-DM (*Cross-Industry Standard Process for Data Mining*), estruturada em seis etapas:

1. **Entendimento do negócio:** definição do problema, dos objetivos e dos critérios de sucesso.
2. **Entendimento dos dados:** análise da estrutura, das variáveis e das características da base.
3. **Preparação dos dados:** avaliação da qualidade dos dados e preparação para as análises.
4. **Modelagem:** aplicação de técnicas estatísticas para investigar associações e relevância das variáveis.
5. **Avaliação:** interpretação dos resultados e validação das conclusões em relação ao problema de negócio.
6. **Implantação:** elaboração de um plano de ação e acompanhamento dos indicadores.

A base utilizada contém informações de 1.470 funcionários e 19 possíveis fatores relacionados ao turnover. Conforme o estudo original, os dados disponibilizados já estavam tratados, não sendo necessária uma etapa adicional de limpeza.

## Análises realizadas

### 1. Análise exploratória de dados

Foram analisadas as características dos colaboradores e a distribuição dos desligamentos, utilizando estatísticas descritivas, tabelas de frequência e visualizações.

As variáveis quantitativas também foram agrupadas em faixas para facilitar a comparação entre grupos e a interpretação das taxas de turnover.

<img width="1739" height="645" alt="image" src="https://github.com/user-attachments/assets/0957864e-a55b-4753-b15b-291ded164f28" />

### 2. Análise bivariada

Foram investigadas as taxas de desligamento em diferentes grupos de funcionários, buscando identificar categorias com maior incidência de turnover e possíveis padrões relevantes para o negócio.

<img width="594" height="484" alt="image" src="https://github.com/user-attachments/assets/4f194f87-2ea1-4127-ad73-baf17d2a8be1" />


### 3. Information Value (IV)

O *Information Value* foi utilizado para avaliar o poder discriminatório das variáveis em relação à saída dos funcionários.

Essa análise ajudou a priorizar as variáveis que apresentaram maior capacidade de distinguir colaboradores que deixaram a empresa daqueles que permaneceram.

<img width="594" height="566" alt="image" src="https://github.com/user-attachments/assets/32315f81-c002-4de4-b41a-a2379be1a373" />

### 4. Análise das relações entre variáveis

Foram investigadas relações entre salário, tempo de carreira e realização de horas extras, buscando compreender como esses fatores se relacionavam com os desligamentos.

Também foi avaliada a relação entre salário e tempo de carreira por meio de regressão e do coeficiente de determinação (R²).

### 5. Visualização e acompanhamento

Os resultados foram organizados em tabelas, gráficos e indicadores, com a utilização do Power BI para apoiar a interpretação dos resultados e o acompanhamento periódico do turnover.

## Principais resultados

A análise exploratória identificou os seguintes resultados:

| Indicador | Resultado |
|---|---:|
| Total de funcionários | 1.470 |
| Funcionários desligados | 237 |
| Taxa de turnover | 16,12% |
| Meta de turnover proposta | 10% |
| Diferença em relação à meta | 6,12 pontos percentuais |

A taxa observada de 16,12% ficou acima da meta de 10% estabelecida para o estudo, indicando uma oportunidade de melhoria na retenção de colaboradores.

### Variáveis de maior relevância

O cálculo do Information Value destacou três variáveis classificadas como de forte poder discriminatório:

- **Salário:** funcionários com salários inferiores a R$ 2.500 apresentaram maior taxa de desligamento.
- **Horas extras:** a realização de horas extras esteve associada a diferenças nas taxas de turnover.
- **Tempo de carreira:** funcionários com tempo de carreira entre 0 e 2 anos apresentaram maior taxa de desligamento.

Esses resultados indicam grupos e fatores que merecem atenção prioritária nas políticas de Recursos Humanos.

### Relação entre salário e tempo de carreira

A análise também identificou uma relação relevante entre salário e tempo de carreira, com coeficiente de determinação (R²) de 71% no estudo apresentado.

Esse resultado indica que, no contexto da análise realizada, o tempo de carreira esteve associado a uma parcela expressiva da variação salarial observada.

### Diferenças salariais entre os grupos

| Indicador | Desligados | Permaneceram |
|---|---:|---:|
| Salário médio | R$ 4.787,09 | R$ 6.832,74 |
| Salário mediano | R$ 3.202,00 | R$ 5.204,00 |

Os funcionários que deixaram a empresa apresentaram médias e medianas salariais inferiores às dos funcionários que permaneceram.

Essa diferença reforça a importância de investigar as políticas de remuneração, sem pressupor que o salário, isoladamente, seja a causa dos desligamentos.

## Plano de ação

Com base nos resultados, foi proposta a utilização da ferramenta 5W2H para organizar as iniciativas de melhoria.

As principais frentes de investigação e atuação são:

- **Remuneração:** avaliar a competitividade salarial e os critérios de progressão na carreira.
- **Jornada de trabalho:** investigar a frequência, os motivos e os impactos das horas extras.
- **Retenção de novos profissionais:** compreender as dificuldades enfrentadas por funcionários em início de carreira.
- **Desenvolvimento profissional:** avaliar oportunidades de capacitação, crescimento e promoção.
- **Monitoramento:** acompanhar mensalmente a taxa de turnover e os indicadores relacionados durante 12 meses, revisando as ações conforme os resultados.

A implementação dessas iniciativas deve considerar o contexto da organização, os recursos disponíveis e a validação dos fatores identificados.

## Indicadores de acompanhamento

Para avaliar os resultados das ações propostas, recomenda-se acompanhar:

- Taxa mensal e acumulada de turnover.
- Quantidade de desligamentos voluntários e involuntários, quando disponível.
- Turnover por faixa salarial e tempo de carreira.
- Turnover entre funcionários que realizam horas extras.
- Evolução dos indicadores antes e depois da implementação das ações.
- Progresso em relação à meta de 10%.

## Conclusão

O projeto demonstra como a análise de dados pode apoiar decisões estratégicas na área de Recursos Humanos.

A combinação de Excel, Python e Power BI permitiu organizar os dados, investigar padrões de desligamento e comunicar os principais resultados. A análise destacou salário, horas extras e tempo de carreira como variáveis prioritárias para investigação e possíveis intervenções.

Os resultados podem subsidiar políticas de remuneração, melhoria das condições de trabalho e desenvolvimento profissional, contribuindo para a retenção de talentos, a preservação do conhecimento organizacional e a redução dos custos associados à rotatividade.

É importante ressaltar que associações estatísticas não comprovam causalidade. A eficácia das ações propostas deverá ser avaliada por meio de acompanhamento contínuo e validação dos resultados no contexto real da organização.

## Referências

- Oliveira, Mairon Henrique de. *Análise de dados para diminuição de Turnover*. Medium, 28 abr. 2024.
- Escola Preditiva.ai. Materiais sobre a metodologia CRISP-DM e análise de dados.
- Thebilab. *Information Value (IV): O que é, Como Calcular e sua Importância para a Análise de Dados*.
- SEBRAE. Material de referência sobre a ferramenta 5W2H.

## Tecnologias

- Excel
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Power BI
- CRISP-DM
- Information Value (IV)
- Análise Exploratória de Dados (AED)

## Autor

**Mairon Henrique de Oliveira**

- **LinkedIn:** [linkedin.com/in/maironhenriquedeoliveira](https://www.linkedin.com/in/maironhenriquedeoliveira)

---

**Objetivo do projeto:** transformar dados em informações úteis para apoiar decisões de Recursos Humanos e contribuir para a redução do turnover.

## Artigo completo

Para conferir a análise completa, os gráficos, os resultados e o plano de ação proposto, acesse o artigo original no Medium:

[**Análise de Dados para Diminuição de Turnover — Mairon Henrique de Oliveira**](https://medium.com/@maironhenrique/an%C3%A1lise-de-dados-para-diminui%C3%A7%C3%A3o-de-turnover-95c010458b0b)
