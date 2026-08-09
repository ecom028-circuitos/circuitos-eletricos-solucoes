# Circuitos Elétricos — Repositório de Soluções
### ECOM028 — Engenharia de Computação — 2026.2

Este repositório reúne, de forma colaborativa, as resoluções produzidas pela
turma para o banco de questões do livro-texto adotado na disciplina. O
processo tem duas fases:

## Fase 1 — Construção do repositório (semanal, um capítulo por vez)

- A cada semana, um novo capítulo do livro-texto é trabalhado.
- Cada aluno resolve **1 a 3 questões** desse capítulo e submete sua
  resolução seguindo a estrutura de pastas abaixo.
- Cada resolução deve indicar **quais conceitos da lista oficial do
  capítulo** (ver pasta `conceitos/`) foram efetivamente trabalhados na
  questão.
- Monitores da disciplina revisam uma **amostra** das entregas semanais
  como controle de qualidade — nem toda entrega passa por correção
  individual, mas todas ficam registradas.

## Fase 2 — Questão de referência (ao final do conteúdo)

- Para cada capítulo, **duas duplas** propõem/adaptam uma questão de
  referência que cubra todos os conceitos da lista oficial — tanto na
  solução algébrica quanto na análise via TyphoonSim.
- A dupla vencedora recebe pontuação extra.
- Todos os quatro alunos das duas duplas participantes passam por uma
  apresentação/arguição individual sobre o domínio do conteúdo.

## Estrutura de pastas

    conceitos/                          lista oficial de conceitos por capítulo
    capitulos/
      cap01/
        alunos/
          <matricula>/
            questao-XX/
              enunciado.tex
              solucao.tex
              solucao.pdf
              conceitos.yaml             checklist dos conceitos cobertos
              typhoonsim/
                modelo.tse               arquivo para abrir no TyphoonSim
                instrucoes.md            orientações de uso do modelo
    referencia/
      cap01/
        dupla-A/
        dupla-B/
        vencedora/                       preenchida após a decisão final

### Captura de tela do TyphoonSim (obrigatória)

Toda pasta `typhoonsim/` de uma entrega deve conter, além do arquivo do
modelo (`modelo.tse`) e do roteiro (`instrucoes.md`), **uma captura de
tela** mostrando o esquemático montado e o painel SCADA em execução (com
os valores lidos visíveis nos instrumentos virtuais).

**Como adicionar:**

1. Salve a captura de tela dentro da própria pasta `typhoonsim/`, com um
   nome descritivo (ex.: `captura-scada.png`).
2. No final do `instrucoes.md`, adicione a imagem usando a sintaxe:
```markdown
   ## Captura de tela (esquemático + painel SCADA)

   ![Esquemático e painel de instrumentação](captura-scada.png)
```
3. O nome do arquivo de imagem usado no link precisa ser **idêntico**
   (incluindo maiúsculas/minúsculas) ao nome do arquivo enviado.

Essa captura serve como evidência de que a verificação experimental foi
realizada e facilita a revisão por amostragem pelos monitores, sem que
seja necessário abrir o TyphoonSim para conferir cada entrega.

## Como submeter sua resolução

1. Crie uma nova *branch* com o padrão `capXX-suamatricula-qYY`
   (exemplo: `cap01-22110875-q47`).
2. Adicione sua pasta em `capitulos/capXX/alunos/<sua matrícula>/questao-YY/`
   com todos os arquivos exigidos.
3. Abra um **Pull Request** usando o modelo (*template*) que aparece
   automaticamente.
4. Aguarde a verificação automática (checa se todos os arquivos
   obrigatórios estão presentes e se o `.tex` compila).
5. Um monitor pode revisar seu PR por amostragem — mas mesmo sem revisão
   individual, sua entrega já fica registrada no histórico do repositório.

---

*Dúvidas sobre o processo: procure o professor ou os monitores da
disciplina.*
