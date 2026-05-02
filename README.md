# Agentejax

> Curso prático em PT-BR para você construir do zero seu próprio agente de IA pessoal — em TypeScript, rodando 24/7 no Telegram, com memória, ferramentas e autonomia. Sem framework fechado, sem lock-in, com cada linha sendo sua.

**[Acessar o curso →](https://inematds.github.io/agentejax/)**

---

## O que é

Um curso interativo no formato INEMA.CLUB, dividido em **3 trilhas / 9 módulos / 54 tópicos**, com:

- 🌱 **Trilha 1 · Fundamentos** — do zero até o agente respondendo no Telegram com memória e ferramentas.
- ⚡ **Trilha 2 · Vida do Agente** — comunicação 24/7, streaming, voz, autonomia, reflexão e skills auto-geradas.
- 🛡 **Trilha 3 · Produção** — MCP, aprovações, defesa contra prompt injection, custos, dashboard, hospedagem e testes.

Além das páginas do curso, a landing page tem um **picker interativo** onde você marca as features que quer e baixa um arquivo `.md` com seu blueprint personalizado — pronto pra colar numa IA e pedir o build.

---

## Por que não usar Hermes ou OpenClaw direto?

Existem ótimos frameworks de agente prontos. Comparação honesta entre os dois mais populares e a abordagem deste curso:

| Aspecto | Hermes | OpenClaw | **Agentejax (este curso)** |
|---|---|---|---|
| Linguagem | Python | TypeScript | TypeScript |
| Modelo de uso | Você instala e usa | Você instala e usa | Você **aprende e constrói** |
| Curva inicial | Baixa | Baixa | Média (3 trilhas) |
| Quem entende o código | Time deles | Time deles | **Você** |
| Customização profunda | Fork e mantém | Fork e mantém | Direto no seu repo |
| Memória multi-camada | Sim (4 camadas) | Sim | Sim (3 camadas, T1 M1.2) |
| Skills auto-geradas | Sim (nativo) | Sim (registry) | Opcional (T2 M2.3) |
| Voz | Sim | Sim (mobile) | Opcional (T2 M2.2) |
| Canais de mensagem | 15+ | 22+ | Telegram (extensível) |
| Multi-agente | Limitado | Sim | Out-of-scope (você adiciona) |
| Cliente mobile nativo | Não | Sim | Telegram já é mobile |
| Aprovações de ações | Trust levels | Por comando | Por comando (T3 M3.1) |
| Lock-in | Roadmap deles | Roadmap deles | **Zero** |
| License | MIT | MIT | MIT |
| Quando faz mais sentido | Quero rodar hoje | Quero ecossistema com loja | **Quero entender e ser dono** |

### Use o Agentejax se

- Você quer **entender cada linha** que roda no seu agente
- Vai depender desse agente em tarefas críticas
- Quer trocar de modelo (Claude / GPT / DeepSeek / Ollama) sem dor
- Quer adicionar ferramentas próprias (CRM, banco, ERP) sem mexer em código de terceiros

### Use um pronto se

- Você só quer testar a ideia em 1 hora
- Não quer manter código TypeScript no longo prazo
- Precisa de integrações de mobile nativo prontas
- Não tem interesse em entender como agentes funcionam por dentro

---

## Estrutura do repositório

```
agentejax/
├── index.html                # Landing page com picker e tabela comparativa
├── curso/
│   └── trilha1/
│       ├── index.html        # Index da Trilha 1 — Fundamentos
│       ├── modulo-1-1.html   # Preparação e Ambiente
│       ├── modulo-1-2.html   # Identidade e Memória
│       └── modulo-1-3.html   # Cérebro e Ferramentas
├── README.md
└── LICENSE
```

Trilhas 2 e 3 chegam nas próximas iterações.

---

## Rodar localmente

Site totalmente estático, sem build. Basta abrir o `index.html` no navegador, ou servir com qualquer servidor HTTP:

```bash
# Python (vem instalado em quase tudo)
python3 -m http.server 8000

# Node (se preferir)
npx serve .

# Depois abre http://localhost:8000
```

---

## Publicação no GitHub Pages

1. Settings → Pages
2. Source: `Deploy from a branch`
3. Branch: `main` / pasta: `/ (root)`
4. Salvar — em ~1 min o site fica em `https://inematds.github.io/agentejax/`

---

## Roadmap

- [x] Trilha 1 · Fundamentos (3 módulos completos)
- [x] Landing com picker interativo + download de blueprint
- [x] Tabela comparativa Hermes × OpenClaw × Agentejax
- [ ] Trilha 2 · Vida do Agente
- [ ] Trilha 3 · Produção
- [ ] Repositório de código de referência (TypeScript) com cada módulo implementado

---

## License

MIT — faça o que quiser. Bifurca, copia, vende, adapta.
