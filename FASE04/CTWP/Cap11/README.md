# Projeto de Classificação de Grãos de Trigo

## Visão Geral

Este projeto aplica algoritmos de aprendizado de máquina para automatizar a classificação de grãos de trigo em cooperativas agrícolas, substituindo o processo manual atualmente em uso. A classificação automática melhora a eficiência e a precisão, reduzindo o potencial de erro humano.

## Objetivo

Desenvolver um modelo eficaz de aprendizado de máquina para classificar variedades de trigo (Kama, Rosa e Canadian) com base em suas características físicas, utilizando a metodologia CRISP-DM para estruturar o processo de desenvolvimento.

## Conjunto de Dados

### Descrição

Utilizamos o "Seeds Dataset" do UCI Machine Learning Repository, que contém 210 amostras de grãos de trigo pertencentes a três variedades diferentes. Os atributos do conjunto de dados incluem:

- **Área:** Medida da área do grão.
- **Perímetro:** Comprimento do contorno do grão.
- **Compacidade:** Calculada como ( \frac{\text{Perímetro}^2}{\text{Área}} ).
- **Comprimento do Núcleo:** Comprimento do eixo principal da elipse equivalente ao grão.
- **Largura do Núcleo:** Comprimento do eixo secundário da elipse.
- **Coeficiente de Assimetria:** Medida da assimetria do grão.
- **Comprimento do Sulco do Núcleo:** Comprimento do sulco central do grão.

## Metodologia

O projeto seguiu a metodologia CRISP-DM, que inclui as seguintes fases:

1. **Entendimento do Negócio:** Identificar a necessidade de automação no processo de classificação de grãos.
2. **Entendimento dos Dados:** Carregar e explorar o conjunto de dados para compreensão inicial.
3. **Preparação dos Dados:**
  - Verificação de dados ausentes.
  - Escalonamento das características usando Min-Max Scaling.
  - Divisão dos dados em conjuntos de treinamento e teste (70/30).
4. **Modelagem:**
   - Implementação de algoritmos de classificação: KNN, SVM, e Random Forest.
   - Otimização de hiperparâmetros para melhorar o desempenho do modelo.
5. **Avaliação:** Uso de métricas como F1-score, precisão e recall para avaliar o desempenho dos modelos.
1. **Implantação:** Preparação do modelo para integração em ambientes operacionais.

## Resultados

Após comparação, o Random Forest Otimizado foi selecionado como o modelo mais eficaz, com um F1-score elevado indicando um bom equilíbrio entre precisão e recall em todas as classes.

## Limitações e Considerações Éticas

### Limitações

- Tamanho do Conjunto de Dados: O número limitado de amostras pode afetar a capacidade do modelo de generalizar.
- Complexidade do Modelo: Modelos complexos podem ser menos interpretáveis.

### Considerações Éticas

- Impacto no Trabalho: A automação pode afetar empregos, exigindo estratégias de requalificação.
- Transparência e Bias: Garantir que o modelo seja transparente e livre de vieses é crucial para manter a confiança dos usuários.

## Conclusões

A automação da classificação de grãos usando aprendizado de máquina não só aumenta a eficiência, mas também reduz erros, proporcionando um impacto positivo significativo nas operações das cooperativas agrícolas.
