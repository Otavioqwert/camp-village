# camp-village
# 🌿 camp-village

Protótipo de mini jogo de simulação com grama procedural, estações do ano e construções — tudo rodando no browser com WebGL + Canvas 2D.

---

## ✨ O que tem aqui

- **Grama instanciada via WebGL** — 7×7 grid de tiles, 250 lâminas por tile (~12.250 lâminas no total), com animação de vento em shader GLSL
- **Ciclo de estações** — Verão → Outono → Inverno → Primavera, cada um afetando cor, vigor e crescimento da grama
- **Sistema de temperatura** por tile com difusão e bias climático individual
- **Crescimento orgânico** baseado em fertilidade por região, temperatura ideal e peso por altura
- **Reset de primavera** — ao entrar na primavera, toda a grama renasce do zero com altura mínima
- **Sistema de construções** — coloque Vila 🧑‍🦲, Mina 🪨 ou Fazenda 🌱 nos tiles; a grama não cresce onde há construção
- **Sistema de recompensas** — ganhe $100 a cada 9 minutos simulados e $1.000 na chegada da primavera
- **HUD colapsável** com FPS, velocidade, tempo simulado, ciclo atual, heatmap de temperatura e barra de vigor

---

## 🚀 Como rodar

Sem dependências! Só abrir o arquivo no browser:

```bash
# Qualquer servidor local funciona, por exemplo:
npx serve .
# ou simplesmente abrir o arquivo direto:
open simulador_grama_estacoes.html
```

> Requer browser com suporte a WebGL 1.0 (Chrome, Firefox, Edge — tudo certo).

---

## 🎮 Controles

| Ação | Como |
|---|---|
| Selecionar tile | Clique no tile |
| Colocar construção | Escolha uma ferramenta (Vila/Mina/Fazenda) e clique no tile |
| Desativar ferramenta | Clique novamente no botão ativo |
| Velocidade da simulação | Botões ⏱ 1× / ⚡ 10× / 🔥 60× |
| Expandir/recolher HUD | Botão ▼/▲ no canto superior esquerdo |
| Coletar recompensa | Clique nos botões pulsantes no canto superior direito |

---

## 🛠 Stack

- **Three.js r128** — renderização instanciada WebGL das lâminas de grama
- **Canvas 2D** (nativo) — chão isométrico, construções e HUD
- **Vanilla JS** — zero frameworks, zero build step

---

## 📁 Estrutura

```
camp-village/
├── simulador_grama_estacoes.html   # Tudo em um único arquivo
└── README.md
```

---

## 🔮 Próximos passos (ideias)

- [ ] Mais tipos de construção com efeitos únicos na grama
- [ ] Sistema de recursos (pedra, madeira, trigo)
- [ ] Eventos climáticos (chuva, seca, geada)
- [ ] Save/load do estado do mapa
- [ ] Modo mobile com touch

---

> Protótipo em desenvolvimento ativo — contribuições e sugestões são bem-vindas!
