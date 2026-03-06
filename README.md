# ⚡ LifeRPG — Evolua sua Vida

Sistema de gamificação da vida real, inspirado em RPGs e no estilo visual de Solo Leveling.

## 🚀 Como Rodar

### Pré-requisitos
- Node.js 18+ (https://nodejs.org)
- npm 9+

### Instalação

```bash
# Entrar na pasta do projeto
cd liferpg

# Instalar dependências
npm install

# Iniciar o servidor de desenvolvimento
npm run dev
```

A aplicação abrirá em: **http://localhost:5173**

### Build para Produção

```bash
npm run build
npm run preview
```

---

## 🗂️ Estrutura do Projeto

```
src/
├── components/
│   ├── Avatar/
│   │   ├── Avatar.jsx          # Avatar SVG animado
│   │   └── AvatarEditor.jsx    # Editor de aparência
│   ├── Dashboard/
│   │   └── Dashboard.jsx       # Tela principal
│   ├── Missions/
│   │   └── Missoes.jsx         # Sistema de missões
│   ├── Workout/
│   │   └── Treinos.jsx         # Sistema de treinos
│   ├── Shop/
│   │   └── Loja.jsx            # Loja de itens
│   ├── Inventory/
│   │   └── Inventario.jsx      # Inventário e equipamentos
│   ├── Gallery/
│   │   └── Galeria.jsx         # Galeria de progresso
│   ├── Profile/
│   │   ├── Perfil.jsx          # Perfil do usuário
│   │   └── Onboarding.jsx      # Tela de boas-vindas
│   └── shared/
│       ├── NavBar.jsx          # Navegação inferior
│       ├── Modal.jsx           # Componente de modal
│       ├── BarraXP.jsx         # Barra de experiência
│       ├── RankBadge.jsx       # Badge de rank
│       └── Notificacoes.jsx    # Sistema de notificações
├── hooks/
│   └── useGameState.js         # Estado global do jogo
├── data/
│   ├── items.json              # Itens da loja
│   └── defaultMissions.json    # Missões padrão
├── utils/
│   ├── xpSystem.js             # Cálculos de XP
│   ├── rankSystem.js           # Sistema de ranks
│   └── economySystem.js        # Sistema econômico
└── styles/
    └── globals.css             # Estilos globais
```

---

## ⚙️ Sistemas

### Sistema de XP
- Crescimento progressivo por nível
- Bônus por streak de dias
- Notificações ao subir de nível

### Sistema de Ranks
| Rank | Nome | XP Mínimo |
|------|------|-----------|
| E | Iniciante | 0 |
| D | Aprendiz | 500 |
| C | Disciplinado | 2.000 |
| B | Avançado | 6.000 |
| A | Elite | 15.000 |
| S | Mestre | 35.000 |
| SS | Lendário | 75.000 |
| SSS | Transcendente | 150.000 |

### Dificuldades de Missão
| Dificuldade | XP | Ouro |
|-------------|-----|------|
| Fácil | 20 | 10 |
| Médio | 40 | 20 |
| Difícil | 80 | 40 |
| Épico | 150 | 75 |

### Streak Bônus
| Streak | Bônus |
|--------|-------|
| 3+ dias | +10% XP |
| 7+ dias | +25% XP |
| 14+ dias | +50% XP |
| 30+ dias | +100% XP |

---

## 💾 Dados

Todos os dados são salvos automaticamente no **localStorage** em formato JSON.

Chave principal: `liferpg_state`

---

## 🎨 Estilo Visual

Inspirado na interface de Solo Leveling System UI:
- Tema escuro (#0f172a)
- Azul neon (#38bdf8) como cor principal
- Fontes Orbitron + Rajdhani
- Animações suaves com CSS
- Efeito glow em elementos importantes

---

## 📱 Funcionalidades

- ✅ Sistema de perfil com foto
- ✅ Avatar personalizável (pele, cabelo)
- ✅ Dashboard com stats completos
- ✅ Missões (criar, editar, concluir, deletar)
- ✅ Treinos com lista de exercícios
- ✅ Loja com 16 itens em 4 categorias
- ✅ Inventário com equipamentos
- ✅ Galeria de progresso (base64)
- ✅ Sistema de streak com bônus
- ✅ Sistema de rank com 8 níveis
- ✅ Notificações em tempo real
- ✅ 100% em português
- ✅ Dados no localStorage (sem backend)
