# 🤖 Meu Mentor

> Seu mentor pessoal com Inteligência Artificial para aprender tecnologia, IA, economia e dados — com a [DIO](https://dio.me) como trilha.

O **Meu Mentor** é um agente de IA que acompanha você na sua jornada de estudos. Ele conhece o seu perfil (objetivos, rotina, nível e progresso) e também as experiências da DIO (Bootcamps, Formações, Cursos, Desafios e muito mais). Com isso, ajuda você a estudar, praticar e planejar os próximos passos.

Este projeto é um fork do **DIO Agent**, mantendo o conhecimento e as skills da DIO e adicionando uma camada pessoal em `agent/knowledge/meu-perfil.md`.

Você não precisa saber programar nem instalar nada complicado. Em **3 passos**, o seu mentor está pronto para usar.

---

## ✨ Três palavras para começar

- 🧠 **Agente de IA:** um chatbot responde perguntas. Um *agente* vai além: lê, planeja e executa passos para ajudar você a alcançar um objetivo. É a diferença entre alguém que explica o caminho e alguém que caminha junto com você.
- 🖥️ **Harness:** é o programa onde o agente roda. O agente é o mentor, e o harness é a sala onde vocês se encontram. O mesmo mentor atende em salas diferentes, por isso o Meu Mentor funciona em vários harnesses.
- 🧩 **Skill:** é uma habilidade do agente, descrita em um guia passo a passo. Você não precisa chamar a skill: o agente percebe o que você precisa e usa a certa sozinho.

Esses e outros termos estão no [Glossário](docs/glossary.md).

---

## 🚀 Comece em 3 passos

### 1️⃣ Instale um harness

Recomendamos o **Google Antigravity**, que tem limites de uso generosos para quem está começando. Mas qualquer harness da lista funciona: escolha um e siga a instalação da documentação oficial dele.

| Harness | Documentação oficial |
|---------|----------------------|
| Google Antigravity (recomendado) | https://antigravity.google/docs |
| Claude Code | https://code.claude.com/docs |
| Codex | https://developers.openai.com/codex |
| OpenCode | https://opencode.ai/docs |
| Hermes | https://hermes-agent.nousresearch.com/docs |

### 2️⃣ Baixe o Meu Mentor e abra no harness

Baixe este repositório do jeito mais simples para você:

- **Com Git:** no terminal, rode `git clone https://github.com/ccostaeconomia/dio-agent.git`
- **Sem Git:** no topo desta página, clique no botão verde **Code**, depois em **Download ZIP**, e extraia a pasta.

Depois, abra no harness a pasta do projeto, a que tem o arquivo `AGENTS.md`. O harness lê esse arquivo sozinho, e o agente já sabe quem é: o seu mentor pessoal de estudos.

### 3️⃣ Preencha seu perfil e converse

Abra `agent/knowledge/meu-perfil.md` e preencha o que souber: objetivos, rotina, nível e o que está estudando. Não precisa ser tudo de uma vez — o agente pode completar o restante conversando com você.

Depois, fale naturalmente, com as suas palavras. Nas primeiras vezes, vale usar um dos [modelos de prompt](#-modelos-de-prompt) abaixo: quanto mais contexto você dá, melhor o agente ajuda.

---

## 🧩 As skills do agente

| Skill | Para que serve | Experimente pedir |
|-------|----------------|-------------------|
| [Sessão de estudo](skills/study-session/SKILL.md) | Conduz uma sessão focada, com objetivo único e prática ativa | "Tenho 40 minutos agora, me ajuda a estudar?" |
| [Revisão semanal](skills/weekly-review/SKILL.md) | Revisa a semana, celebra avanços e define as próximas metas | "Vamos revisar minha semana?" |
| [Plano de estudos](skills/study-plan/SKILL.md) | Organiza o que estudar, em que ordem e em quanto tempo | "Quero concluir este Bootcamp em 2 meses, me ajuda?" |
| [Destravar desafio](skills/unblock-challenge/SKILL.md) | Conduz você até a solução de um desafio, sem dar a resposta pronta | "Travei nesse desafio, me ajuda?" |
| [Explicar conceito](skills/explain-concept/SKILL.md) | Explica conceitos de forma simples, com analogias e exemplos | "Não entendi o que é uma API." |
| [Pesquisa na web](skills/web-search/SKILL.md) | Responde dúvidas atuais (versões, lançamentos, mercado) com fontes citadas | "Qual a versão estável do Node hoje?" |
| [Revisão de portfólio](skills/portfolio-review/SKILL.md) | Dá feedback sobre o seu portfólio e GitHub antes de buscar vagas | "O que falta no meu GitHub para uma vaga júnior?" |
| [Caminho AI Builder](skills/ai-builder-path/SKILL.md) | Ajuda você a escolher o próximo passo na Carreira AI Builder | "Qual Formação AI Builder combina comigo?" |

A pesquisa na web usa a busca do seu harness. Se ele não tiver busca própria, veja [como conectar o You.com](docs/youcom-mcp.md), que tem uma opção gratuita.

---

## 📝 Modelos de prompt

Copie, preencha o que está entre colchetes e envie. Não precisa de formato perfeito: o agente pede mais detalhes se precisar.

**⏱️ Sessão de estudo**

```
Quero fazer uma sessão de estudo agora.
- Tempo disponível: [ex: 40 minutos]
- O que quero estudar: [ex: revisar funções em JavaScript]
- Meu objetivo com isso: [ex: entender o que é uma função e praticar]
- Como estou me sentindo: [ex: cansado, animado, sem foco]
```

**📅 Revisão semanal**

```
Vamos revisar minha semana.
- O que eu queria ter feito: [cole as metas da semana]
- O que eu realmente fiz: [resumo rápido]
- O que atrapalhou: [ex: trabalho, falta de tempo, dúvida travada]
- O que funcionou bem: [ex: estudar de manhã, praticar com projetos]
```

**🗺️ Plano de estudos**

```
Quero montar um plano de estudos.
- Meu objetivo: [ex: ser dev back-end, concluir um Bootcamp]
- O que quero fazer na DIO: [link ou nome do Bootcamp, Formação, Aceleração ou Carreira]
- O que já tenho: [um plano de ação ou de estudos, se tiver]
- Meu nível hoje: [iniciante, intermediário, avançado]
- Tempo disponível: [ex: 1 hora por dia, de segunda a sexta]
```

**🔓 Destravar desafio**

```
Estou travado em um Desafio de [Código, Projeto ou Criativo] da DIO.
- O que o desafio pede: [cole o enunciado ou, no Desafio de Projeto, o link do repositório do desafio]
- Onde eu travei: [explique o ponto da dificuldade]
- Meu código ou repositório: [cole o código ou o link, se tiver]
Me ajuda a destravar sem dar a resposta pronta.
```

**💡 Explicar conceito**

```
Me explica o conceito de [ex: API, laço de repetição, herança].
- Meu nível: [nunca vi, já ouvi falar, quero aprofundar]
```

**🧭 Caminho AI Builder**

```
Quero escolher meu próximo passo na Carreira AI Builder.
- O que quero construir com IA: [ex: um produto para o meu negócio, um software, agentes que automatizam processos, ainda não sei]
- Minha experiência com programação: [nenhuma, o básico, trabalho com desenvolvimento]
- Meu objetivo: [ex: mudar de carreira, tirar uma ideia do papel]
```

---

## 🎨 Personalize o seu mentor

Quer mudar o nome, o tom ou o foco do agente? Estes são os arquivos certos:

| O que mudar | Arquivo |
|-------------|---------|
| Nome, identidade e missão | `AGENTS.md` |
| Personalidade e tom de voz | `agent/persona.md` |
| Objetivos, rotina, nível e progresso | `agent/knowledge/meu-perfil.md` |
| Conhecimento sobre a DIO | `agent/knowledge/dio-platform.md` e `learning-experiences.md` |
| Skills (o que o agente sabe fazer) | `skills/<nome>/SKILL.md` |

Para criar uma skill nova, siga o guia em [skills/README.md](skills/README.md).

---

## 🔄 Mantenha o Meu Mentor atualizado

O projeto evolui com o tempo. Se você usou Git, rode `git pull` no terminal, dentro da pasta (ou peça para o próprio agente rodar). Se baixou o .zip, baixe de novo.

Atenção: se você personalizou os arquivos e rodar `git pull`, podem aparecer conflitos. Nesse caso, resolva mantendo as suas mudanças ou copie o que interessa da versão nova.

---

## 🗂️ Estrutura do repositório

```
dio-agent/
├── README.md                Este guia
├── AGENTS.md                Definição do agente (lida pelo harness)
├── CLAUDE.md                Atalho para o Claude Code
├── agent/
│   ├── persona.md           A personalidade e o tom do agente
│   └── knowledge/
│       ├── meu-perfil.md    Seus objetivos, rotina, nível e progresso
│       ├── dio-platform.md  O que é a DIO e como ela funciona
│       └── learning-experiences.md  Tipos de experiência da DIO
├── skills/                  Uma pasta por skill, cada uma com o seu SKILL.md
│   ├── study-session/       Sessão de estudo guiada
│   ├── weekly-review/       Revisão semanal
│   ├── study-plan/          Plano de estudos
│   ├── unblock-challenge/   Destravar desafio
│   ├── explain-concept/     Explicar conceito
│   ├── web-search/          Pesquisa na web
│   ├── portfolio-review/    Revisão de portfólio
│   └── ai-builder-path/     Caminho AI Builder
└── docs/
    ├── glossary.md          Glossário de termos
    └── youcom-mcp.md        Como conectar a busca do You.com
```

---

## 🤝 Contribua

Tem uma ideia de skill? Veja [como criar uma skill](skills/README.md) e abra um pull request no seu fork.

---

## 💬 Sobre este projeto

O Meu Mentor foi criado a partir do DIO Agent para acompanhar você nos seus estudos, dentro e fora da DIO. A ideia é simples: aprender na era da IA fica mais fácil quando você tem um mentor que conhece os seus objetivos e está disponível a qualquer hora.

Bons estudos! 🚀
