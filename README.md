# 💻 ADS — Workspace & VS Code Setup

![Preview](IMG/VSCode.png)

> Ambiente de desenvolvimento em execução — VS Code + WSL2 + SynthWave '84

---

## 📌 Sobre o Projeto

Ambiente de desenvolvimento estruturado para a graduação em **Análise e Desenvolvimento de Sistemas (ADS)**.

Todo o código reside fisicamente no filesystem do **Fedora Linux 43 (WSL2)**, garantindo velocidades de compilação nativas. A interface é renderizada pelo **VS Code no Windows** via extensão WSL — eliminando os gargalos de I/O do NTFS sem abrir mão do ambiente gráfico do Windows.

---

## 🖥️ Ambiente

| Componente | Detalhe |
|---|---|
| **CPU** | Intel Core i3-10100 @ 3.60 GHz (8 threads) |
| **RAM** | 16 GB DDR4 |
| **GPU** | NVIDIA GeForce RTX 3050 + Intel UHD 630 |
| **OS** | Windows 11 Pro (25H2) + Fedora 43 WSL2 |
| **Editor** | VS Code via WSL Extension |
| **Compilador** | GCC (`/usr/bin/gcc`) |
| **Debugger** | GDB (`/usr/sbin/gdb`) |
| **Tema** | SynthWave '84 com Neon Glow |
| **Ícones** | Material Icon Theme |
| **Shell** | Zsh 5.9 + Starship |

---

## ⚙️ Stack

| Ferramenta | Função |
|---|---|
| VS Code + WSL Extension | Editor integrado ao Linux |
| Fedora Linux 43 (WSL2) | Filesystem e compilação |
| GCC | Compilador C/C++ |
| SynthWave '84 + Custom CSS | Tema com efeito neon/glow |
| Starship | Prompt do terminal integrado |

---

## 📁 Estrutura do Diretório

```text
VSCode/  (/home/kadota/VSCode)
├── .vscode/
│   ├── launch.json       ← Configurações de debug
│   └── tasks.json        ← Tasks de compilação (GCC)
├── Algoritmos/           ← Disciplina: Algoritmos
├── Lógica de Programação/ ← Disciplina: Lógica de Programação
├── IMG/
│   └── VSCode.png
├── .gitignore
└── README.md
```

---

## 🔄 Restauro Pós-Formato

### 1 — Clonar o repo
```bash
git clone https://github.com/matheuskadota/ADS_VSCode-Setup /home/kadota/VSCode
```

### 2 — Abrir no VS Code
```bash
code /home/kadota/VSCode
```

### 3 — Extensões WSL (Fedora Linux 43) — 8 extensões
Instalar no VS Code após conectar ao WSL:

- C/C++ (Microsoft)
- C/C++ DevTools (Microsoft)
- C/C++ Extension Pack (Microsoft)
- C/C++ Themes (Microsoft)
- CMake Tools (Microsoft)
- Code Runner (Jun Han)
- GitHub Copilot Chat (GitHub)
- Portuguese (Brazil) Language Pack (Microsoft)

### 3b — Extensões Local (Windows) — 7 extensões
Instalar no VS Code local (não no WSL):

- C/C++ Themes (Microsoft)
- Custom CSS and JS Loader (be5invis)
- Error Lens (Alexander)
- Material Icon Theme (Philipp Kief)
- Portuguese (Brazil) Language Pack (Microsoft)
- SynthWave '84 (Robb Owen)
- WSL (Microsoft)

### 4 — Reativar o glow do SynthWave
Após instalar as extensões:
1. `Ctrl+Shift+P` → `SynthWave '84: Enable Neon Dreams`
2. `Ctrl+Shift+P` → `Enable Custom CSS and JS`
3. Reiniciar o VS Code como administrador

---

## 📝 Convenção de Nomes

Cada disciplina organiza seus arquivos por aula:

```text
Algoritmos/
├── Aula01_variaveis.c
├── Aula02_condicionais.c
└── Aula03_loops.c
```
