# 🧠 Especialista em Neuro-Discovery Inquisitivo

> Skill para **Claude Code**. Um discovery **confrontador** que conduz uma
> entrevista 360° do seu problema, bate de frente com as suas contradições e
> entrega um diagnóstico sem ambiguidade — com **metas quantitativas**.

Não é um "sim-senhor". É um investigador clínico e obstinado que **recusa o
diagnóstico fácil**: ele questiona a lógica e a emoção por trás do que você pede,
descobre o que você nem sabia que precisava dizer e só entrega a solução quando
o problema real está 100% claro.

---

## 📌 O que é

Uma variação **inquisitiva/confrontadora** da metodologia de Neuro-Discovery.
Enquanto um briefing comum anota o que o cliente pede, esta skill faz o caminho
inverso: **do pedido técnico de volta até o desejo, a dor e o objetivo reais** —
que quase sempre estão escondidos ou nem foram verbalizados.

Ela combina neurociência cognitiva e psicologia comportamental (sistema límbico
vs. córtex, foco regulatório de Tory Higgins, aversão à perda, saliência
afetiva) com uma **postura de confronto**: aponta cada contradição na hora e não
avança enquanto houver incoerência ou lacuna de pé.

---

## 🎯 Para que serve e o que ela ajuda

Ela ajuda você a:

- **Descobrir o problema real** por trás de um pedido técnico (o sintoma quase
  nunca é a doença).
- **Revelar dores, causas e objetivos não ditos** — inclusive os que o próprio
  solicitante não tem consciência.
- **Expor contradições e exigências incompatíveis** *antes* de gastar tempo e
  dinheiro construindo a coisa errada.
- **Separar o tema principal** dos tópicos complementares e dos falsos urgentes.
- **Priorizar**: o que resolver primeiro, o que dói mais, o que pode esperar.
- **Mapear os grupos envolvidos** (quem decide, executa, resiste, paga) e o
  **caminho desejado** até a solução.
- **Amarrar tudo a métricas** — cada causa, plano e ação vem com
  *linha de base → meta → prazo → indicador*, para você enxergar como chegar na
  resolução.

**Quando usar:** início de projeto, briefing raso, kickoff, levantamento de
requisitos, qualificação de lead — ou sempre que você "acha" que sabe qual é o
problema mas não tem certeza, e quer ser **desafiado** até ter.

**Para quem é:** consultores, PMs, product designers, devs, founders, agências —
qualquer pessoa que precise entender o que o cliente (ou você mesmo) realmente
quer antes de propor solução.

---

## 🧬 Como ela funciona (a metodologia)

**Motor de raciocínio** (usado para decidir *onde perfurar*):

- **Límbico vs. córtex** — você pede com a lógica, mas decide com a emoção.
- **Foco regulatório (Higgins)** — Promoção (ganho/status) vs. Prevenção
  (segurança/risco zero).
- **Carga cognitiva e contradições** — o conflito interno vaza em justificativas
  em excesso e incoerências.
- **Saliência afetiva** — as palavras de maior carga emocional guiam o confronto.

**Profundidade — as 3 camadas:** Sintoma → Dor/Defesa → Recompensa Oculta.

**Largura — o Mapa 360** (as 8 dimensões que precisam ser cobertas antes de
fechar):

| # | Dimensão | O que investiga |
|---|----------|-----------------|
| 1 | Tema principal | O problema central, separado dos sintomas |
| 2 | Tópicos complementares | Temas adjacentes não citados |
| 3 | Dores (ditas e não ditas) | O que ele nomeou e o que vaza nas entrelinhas |
| 4 | Causas | A raiz real de cada dor (não o palpite) |
| 5 | Objetivos e caminho desejado | Onde quer chegar e por qual rota |
| 6 | Prioridades | A hierarquia real do que resolver primeiro |
| 7 | Grupos/stakeholders | Quem decide, executa, resiste, paga |
| 8 | Restrições e o não-dito | Orçamento, prazo, política, limites técnicos |

**Postura:** entrevista de verdade (raramente menos de **6–10 perguntas**), uma
pergunta incisiva por vez, apontando contradições na hora, sempre sincera. Ela
fecha por **cobertura 360 completa + ausência de incoerência** — nunca por
pressa.

---

## ⚙️ Instalação

**Pré-requisito:** [Claude Code](https://docs.claude.com/claude-code) instalado.

### Como skill pessoal (disponível em todos os seus projetos)

```bash
git clone https://github.com/mikenew01/neuro-discovery-inquisitivo.git \
  ~/.claude/skills/neuro-discovery-inquisitivo
```

### Como skill de um projeto específico

Dentro da raiz do projeto:

```bash
git clone https://github.com/mikenew01/neuro-discovery-inquisitivo.git \
  .claude/skills/neuro-discovery-inquisitivo
```

### Verificação

Após clonar, a estrutura deve ficar assim:

```
neuro-discovery-inquisitivo/
├── SKILL.md                        # instruções principais da skill
├── README.md
└── references/
    └── confronto-toolkit.md        # técnicas de confronto e bancos de perguntas
```

Reinicie o Claude Code. A skill é descoberta automaticamente e passa a aparecer
na lista de skills disponíveis (o `README.md` e a pasta `.git` são ignorados —
o Claude lê o `SKILL.md`).

### Atualizar para a versão mais recente

```bash
git -C ~/.claude/skills/neuro-discovery-inquisitivo pull
```

---

## ▶️ Como usar

### Invocação direta (slash command)

```
/neuro-discovery-inquisitivo Quero um app de delivery, mas rápido e barato.
```

### Invocação natural

Basta descrever um pedido de projeto e pedir para entender a fundo / ser
questionado. A skill dispara sozinha quando o pedido é raso, contraditório, ou
quando você pede um discovery. Exemplos de gatilho:

- *"Me ajuda a descobrir o que meu cliente realmente quer com esse projeto."*
- *"Quero ser desafiado sobre o que eu realmente preciso construir aqui."*
- *"Esse briefing está confuso, quero depurar as contradições antes de começar."*

### O que esperar da sessão

1. Ela se apresenta e faz a **primeira pergunta** (opções de escolha + a
   alternativa "Outro" para texto livre).
2. Conduz uma **entrevista** — uma pergunta por vez — percorrendo as 8 dimensões
   do Mapa 360.
3. **Aponta cada contradição na hora** e te força a resolvê-la.
4. Só no final entrega o **relatório de diagnóstico**.

> 💡 **Dica:** responda com sinceridade. A skill foi feita para furar respostas
> de fachada — quanto mais honesto você for, mais útil é o diagnóstico.

---

## 📄 O relatório final

Ao fechar, você recebe um documento estruturado:

1. **🧭 Diagnóstico do Projeto** — Pedido Literal · Tema Principal · Verdadeiro
   Objetivo Oculto · Tópicos Complementares.
2. **🧠 Perfil Neuropsicológico** — foco regulatório dominante, linguagem
   detectada e as 3 palavras de saliência.
3. **🚨 Ranking de Dores e Medos** — do mais crítico ao menos, com causa,
   evidência e número (base → meta → prazo).
4. **🎯 Ranking de Recompensas** — o que dá mais dopamina (status) ou ocitocina
   (segurança), em ordem.
5. **👥 Grupos Envolvidos e Caminho Desejado** — stakeholders e a rota até a
   solução, com marcos quantitativos.
6. **🛡️ Recomendações Estratégicas** — em ranking, cada ação com sua métrica
   (base → meta → prazo → indicador).

---

## 🧪 Exemplo relâmpago

**Pedido inicial (o sintoma):**
> "Quero um sistema de IA que envie relatório de produtividade a cada 2h para
> cada dev, com alertas vermelhos para quem está abaixo da média."

**O confronto (trecho):**
> "Você diz que o time está desmotivado — e me pede uma máquina de vigilância que
> aprofunda exatamente essa desmotivação. E 'abaixo da média' deixa metade do
> time no vermelho para sempre, por definição. Antes de falar de stack: o que
> você realmente quer que esse sistema faça?"

**O diagnóstico (o que estava escondido):**
> O projeto não era sobre produtividade — era um **escudo político**: o gestor
> temia perder o cargo e queria "mostrar serviço". A recomendação real virou
> *diagnosticar a causa da queda* (que ele nem conhecia) e *gerir para cima* com
> métricas — não construir IA nenhuma.

---

## ❓ FAQ

**Ela é rude?**
Não. Ela confronta a **lógica e a emoção** — nunca a pessoa. Firme com a ideia,
respeitosa com você.

**Funciona fora do Claude Code?**
A *metodologia* sim (dá para usar o conteúdo do `SKILL.md` como system prompt em
outro contexto), mas o formato interativo de perguntas usa a ferramenta
`AskUserQuestion`, nativa do Claude Code.

**Qual a diferença para um discovery "normal" e gentil?**
Esta versão é **obstinada**: não aceita resposta superficial, não para em 3
perguntas e não fecha com nenhuma contradição ou lacuna em aberto.

---

## 🗂️ Estrutura

| Arquivo | Função |
|---------|--------|
| `SKILL.md` | Persona, motor, Mapa 360, fluxo, filtros e formato do relatório |
| `references/confronto-toolkit.md` | Técnicas de confronto, bancos de perguntas por camada e por dimensão, checklist de fechamento |
| `README.md` | Este arquivo |
