# Otimização de Treliças Utilizando Algoritmos Genéticos

Bem-vindo ao **Projeto de Otimização de Treliças**! Este projeto utiliza o poder dos Algoritmos Genéticos (uma forma de Inteligência Artificial) para projetar a treliça ideal baseada em parâmetros fornecidos. O objetivo é minimizar o peso da treliça, mantendo a integridade estrutural.

## 📜 Contexto do Problema

Treliças são componentes essenciais em muitas estruturas de engenharia, e otimizar seu design pode resultar em significativas economias de material e custo. Neste projeto, focamos em otimizar as áreas das seções transversais das barras e os comprimentos de certas barras da treliça, garantindo que a estrutura atenda aos padrões de segurança e desempenho exigidos.

### Variáveis a Otimizar

- **Áreas das Seções Transversais (A):** A1, A2, A3, ..., A13.
- **Comprimentos das Barras (L):** l1, l2, l3, l4, l6, l8, l10.
- **Vão Livre Mínimo:** 8 metros.

### Propriedades do Material

- **Massa Específica do Aço:** 7870 kg/m³
- **Módulo de Elasticidade:** 200 GPa
- **Coeficiente de Segurança (Sg):** 2
- **Limite de Escoamento do Aço Estrutural ASTM A36 (σE):** 300 MPa

## 🔧 Como Funciona

### Visão Geral do Algoritmo Genético

O Algoritmo Genético (AG) é um heurístico de busca inspirado no processo de seleção natural. Ele é particularmente útil para resolver problemas de otimização com grandes e complexos espaços de busca.

### Etapas Principais

1. **Inicialização:** Geração aleatória da população inicial de designs de treliça.
2. **Avaliação:** Cálculo da aptidão de cada treliça com base no peso e integridade estrutural.
3. **Seleção:** Escolha das melhores treliças para gerar a próxima geração.
4. **Crossover & Mutação:** Combinação e leve alteração dos designs escolhidos para explorar novas soluções.
5. **Iteração:** Repetição do processo até que o algoritmo converja para um design ótimo.

### Critérios de Design da Treliça

O design da treliça deve atender aos seguintes critérios:
- O peso deve ser minimizado, garantindo que a estrutura suporte as cargas aplicadas.
- O design deve manter um vão livre de pelo menos 8 metros.
- Todos os valores de tensão na treliça devem estar dentro dos limites permitidos definidos pelo fator de segurança e propriedades do material.

## 📊 Resultados

![Estrutura da Treliça](https://github.com/user-attachments/assets/b2b8ec93-3353-4804-b150-5cff751d2b7a)

O design otimizado da treliça, gerado pelo Algoritmo Genético, mostra economias significativas de material, mantendo o desempenho estrutural. A figura acima ilustra o design final.

## 🚀 Como Começar

### Pré-requisitos

- Python 3.x
- Bibliotecas Python necessárias (listadas em `requirements.txt`)

### Instalação

Clone o repositório e instale as dependências necessárias:

```bash
git clone https://github.com/kaiqu3santos/IA_Algoritmo-Genetico_Trelica.git
cd IA_Algoritmo-Genetico_Trelica
pip install -r requirements.txt
