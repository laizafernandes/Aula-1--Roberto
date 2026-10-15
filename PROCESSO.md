# PROCESSO.md — Lab 1 · Pisca-LED

**Aluno:** Laiza Fernandes Guimaraes · laiza.guimaraes@sou.inteli.edu.br
**Turma / grupo:** T26 · Grupo 1

## 1. Contextualizar
- **Objetivo:** fazer um LED piscar pra mostrar que o Arduino tá ligado e funcionando.
- **Comportamento esperado:** o LED fica aceso 200 ms e apagado 1800 ms, então pisca uma vez a cada 2 s.
- **Critério de aceitação:** o ciclo medido tem que dar entre 1,9 e 2,1 s, e a corrente no LED tem que ficar abaixo de 20 mA.
- **Delegação à IA × feito sozinho:** vou usar a IA pra entender a conta do resistor. A montagem, o teste e as respostas da etapa 5 eu faço sozinha.

## 2. Consultar
- **Ferramenta:** ChatGPT
- **Pergunta (exata):** que valor de resistor limita a corrente de um LED vermelho ligado a 5 V, e de onde sai essa conta?
- **Resposta resumida:** A conta vem da lei de Ohm. O LED vermelho “consome” uns 2 V, então sobram 3 V no resistor. A corrente é I = (5 − 2) ÷ R. Com 220 Ω, dá 3 ÷ 220 ≈ 0,0136 A, ou seja, uns 13,6 mA. Isso fica abaixo dos 20 mA recomendados, então o LED fica seguro.

## 3. Confrontar
- **Afirmação conferida:** com 220 Ω a corrente fica em torno de 13,6 mA
- **Fonte primária:** Animação da aula
- **Trecho / cálculo:** 3/220 ≈ 13,6 mA.
- **Veredito:** Confirmada
- **ADR:** —

## 4. Construir
- **Wokwi:** https://wokwi.com/projects/477968923692143617
- **Repositório / commit:** https://github.com/laizafernandes/Aula-1--Roberto.git
- **Ciclo medido:** 2.02 s
- **Corrente calculada com 220 Ω:** 13.6 mA
- **Projeto funcionando:** não

## 5. Comprovar (sem IA)
1. **Corrente com 330 Ω:** 9.9 mA — cálculo: I = 5-2/330=3/330=0,00909A
2. **Resistor de 0 Ω:** Porque nada limita a corrente, que passa muito do máximo suportado pelo LED. — —
3. **LED no pino 12:** Só o valor de PINO_LED passa a ser 12 (e o fio vai para o pino 12).
4. **TEMPO_APAGADO para 500 ms a cada 3 s:** 2500 ms

Declaro que respondi a etapa Comprovar sem IA: sim
