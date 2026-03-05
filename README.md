# 💻 ADS Workspace & VS Code Configuration

![Preview](IMG/VSCode.png)

> Preview do ambiente VSCode em execução.

---

## 📌 Sobre o Projeto

Este é o ambiente de desenvolvimento principal estruturado para a graduação em **Análise e Desenvolvimento de Sistemas (ADS)**.

A arquitetura deste workspace foi desenhada para contornar gargalos de I/O de disco tradicionais do Windows. Todo o código e os diretórios de estudo residem fisicamente dentro do sistema de arquivos de uma máquina virtual WSL2 (Fedora Linux 43), garantindo velocidades de compilação nativas, enquanto a interface de usuário (UI) é renderizada de forma fluida pelo VS Code no host Windows.

---

## 🏗️ Estrutura do Diretório

O workspace está dividido em módulos acadêmicos para facilitar a indexação e o versionamento:

\`\`\`text
📦 VSCode (Nativo Linux: /home/usuario/VSCode)
 ┣ 📂 Algoritmos
 ┣ 📂 Lógica de Programação
 ┣ 📂 .vscode (Configurações de Workspace Híbrido)
 ┗ 📜 .gitignore
\`\`\`
