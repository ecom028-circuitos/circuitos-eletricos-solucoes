# Instruções de verificação no TyphoonSim — Questão 01, Capítulo 1

> Ver Capítulo 1 do e-book ("Conhecendo o TyphoonSim") para o passo a passo
> geral de instalação e uso do Schematic Editor / painel SCADA. Este arquivo
> cobre apenas o roteiro específico desta questão.

## Objetivo

Confirmar experimentalmente que, para `Rcarga = 5 Ω`, a potência-alvo que
mantém `Vop` dentro da faixa `[0,90 V ; 1,56 V]` é `Palvo = 250 mW`.

## Montagem sugerida

1. Fonte de tensão CC: `Voc = 1,56 V`.
2. Resistor de carga ajustável: `Rcarga = 5 Ω` (fixo, conforme o exemplo).
3. Inserir um bloco de medição de potência (ou calcular `P = V × I` a partir
   de multímetro de tensão + multímetro de corrente no mesmo ramo).

## Procedimento

1. Compilar o modelo e abrir o painel SCADA.
2. Ajustar a fonte/controle de forma que a potência dissipada em `Rcarga`
   fique em `250 mW`.
3. Ler `Vop` no multímetro virtual.
4. **Resultado esperado:** `Vop ≈ 1,118 V`, dentro da tolerância de medição
   do simulador.
5. **Variação paramétrica (opcional, para consolidar o conceito):** repetir
   o procedimento para `Palvo = 500 mW` e `750 mW`, confirmando que `Vop`
   ultrapassa o teto de `1,56 V` ou sai da faixa admissível — evidenciando
   por que `250 mW` é, de fato, a maior potência-alvo válida.

## Arquivo do modelo

O arquivo `modelo.tse` (a ser criado diretamente no TyphoonSim, salvo nesta
mesma pasta) deve conter a montagem descrita acima, pronta para ser aberta
por qualquer colega que queira reproduzir o experimento.
