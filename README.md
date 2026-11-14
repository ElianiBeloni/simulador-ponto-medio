# Simulador do algoritmo do ponto médio

Rasterização de uma circunferência pelo algoritmo do ponto médio, executada um passo por vez numa grade de pixels.

**Abrir:** https://elianibeloni.github.io/simulador-ponto-medio/

## Como usar

1. Informe o raio `r` e o centro `(X0, Y0)`.
2. Clique em **Iniciar** para marcar o centro e o primeiro ponto.
3. Clique em **Avançar Passo** para calcular o próximo pixel.

A cada passo a página mostra as coordenadas `x`, `y` e o valor da variável de decisão `h_m`.

## O que o simulador mostra

- **Variável de decisão.** Começa em `h_m = 1 - r`. O sinal de `h_m` diz se o ponto médio entre os dois pixels candidatos está dentro ou fora da circunferência, e isso decide qual deles é pintado.
- **Só aritmética inteira.** A atualização de `h_m` usa apenas somas e multiplicações por 2, sem raiz quadrada nem ponto flutuante.
- **Simetria de ordem 8.** O algoritmo calcula um único octante; os outros sete pontos saem por reflexão.

## Executar localmente

Não há dependências nem etapa de build: basta abrir `index.html` no navegador.
