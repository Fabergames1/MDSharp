# 🎮 MDSharp

Emulador e ambiente de análise/debug para Mega Drive / Genesis desenvolvido em C# utilizando .NET 6.

---

# 📌 Sobre o Projeto

O **MDSharp** é um projeto focado na emulação, análise e depuração do hardware do Sega Mega Drive (Genesis).

O sistema implementa diversos componentes do console original, incluindo:

* ⚙️ CPU Motorola 68000
* 🎵 Chip de áudio YM2612
* 🔊 PSG SN76489
* 🖥️ VDP (Video Display Processor)
* 🎮 Controle de entrada
* 💾 Gerenciamento de memória
* 📦 Leitura de ROMs
* 🔍 Ferramentas de debug e tracing
* 🎨 Visualização gráfica da VRAM e paletas

Além da emulação tradicional, o projeto possui ferramentas avançadas de inspeção interna do hardware para fins de estudo, engenharia reversa e desenvolvimento.

---

# 🖼️ Recursos Principais

## 🎮 Emulação do Mega Drive

* Execução de ROMs
* Emulação de CPU Motorola 68000
* Emulação Z80
* Renderização de vídeo
* Processamento de áudio
* Comunicação entre barramentos

## 🔍 Ferramentas de Debug

O projeto possui diversas janelas e ferramentas de análise:

* Visualizador de registradores
* Memory tracing
* Visualizador de código
* Análise de instruções
* Visualização da VDP
* Fluxo de execução
* Monitoramento de IO
* Ferramentas de depuração em tempo real

## 🎵 Sistema de Áudio

Implementação dos chips:

* YM2612 FM Synth
* SN76489 PSG
* Processamento de canais sonoros
* Geração de áudio em tempo real

## 🖥️ Renderização Gráfica

* Renderização baseada em DirectX
* Processamento de sprites
* Renderização por scanline
* Visualização de tiles e patterns
* Gerenciamento de paletas

---

# 🛠️ Tecnologias Utilizadas

## Linguagem

* C#

## Framework

* .NET 6 (Windows)

## APIs e Bibliotecas

* SharpDX
* NAudio
* Windows Forms

---

# 📂 Estrutura do Projeto

```bash
MDSharp/
├── Form_Main.cs
├── md_main.cs
├── md_m68k.cs
├── md_z80.cs
├── md_vdp.cs
├── md_music.cs
├── md_bus.cs
├── md_cartridge.cs
├── md_io.cs
├── Form_Code.cs
├── Form_Registry.cs
├── Form_VDP_Screen.cs
└── Form_MUSIC.cs
```

---

# ⚙️ Componentes Implementados

## 🧠 CPU Motorola 68000

Arquivos principais:

* `md_m68k.cs`
* `md_m68k_memory.cs`
* `md_m68k_addressing.cs`
* `md_m68k_sub.cs`

Recursos:

* Decodificação de instruções
* Addressing modes
* Controle de memória
* Operações aritméticas
* Fluxo de execução

---

## 🎵 Sistema de Som

Arquivos principais:

* `md_music.cs`
* `md_music_ym2612_core.cs`
* `md_music_sn76489_core.cs`

Recursos:

* Emulação FM
* PSG
* Geração de canais
* Reprodução em tempo real

---

## 🖥️ Video Display Processor (VDP)

Arquivos principais:

* `md_vdp.cs`
* `md_vdp_renderer.cs`
* `md_vdp_dma.cs`

Recursos:

* Renderização de tiles
* Sprites
* DMA
* Scanlines
* Frame rendering
* VRAM handling

---

# 🧪 Ferramentas Integradas

## 📜 Code Viewer

Permite:

* Visualizar instruções
* Fazer tracing
* Acompanhar execução
* Analisar registradores

## 🎨 Pattern Viewer

Visualização de:

* Tiles
* Patterns
* Paletas
* VRAM

## 🔊 Audio Monitor

Ferramentas para:

* Monitoramento do YM2612
* Monitoramento PSG
* Visualização de registradores de áudio

---

# ▶️ Como Executar

## Pré-requisitos

* Windows 10 ou superior
* .NET 6 SDK
* Visual Studio 2022

---

## 🔧 Compilação

Clone o repositório:

```bash
git clone https://github.com/seu-usuario/MDSharp.git
```

Abra a solução no Visual Studio.

Compile em:

```bash
Release
```

ou

```bash
Debug
```

---

# 📦 Dependências

O projeto utiliza:

```bash
SharpDX
NAudio
```

Dependências já configuradas no projeto `.csproj`.

---

# 🎮 Compatibilidade

O projeto foi desenvolvido para:

* Windows x64
* .NET 6

---

# 📸 Interface

O MDSharp possui múltiplas janelas especializadas:

* Main Window
* Registry Viewer
* VDP Screen Viewer
* Pattern Viewer
* Palette Viewer
* Code Analyzer
* Flow Viewer
* Audio Monitor

---

# 📈 Objetivos do Projeto

O projeto foi criado para:

* Estudo de arquitetura do Mega Drive
* Engenharia reversa
* Pesquisa em emulação
* Desenvolvimento de ferramentas de debug
* Aprendizado sobre hardware clássico

---

# 🚀 Melhorias Futuras

* Compatibilidade ampliada de ROMs
* Melhor sincronização de áudio
* Otimizações gráficas
* Debugger avançado
* Save states
* Suporte a shaders
* Ferramentas de profiling
* Interface modernizada

---

# 🤝 Contribuição

Contribuições são bem-vindas.

## Fluxo recomendado

```bash
# Fork do projeto

# Criar branch

git checkout -b feature/minha-feature

# Commit

git commit -m "feat: nova funcionalidade"

# Push

git push origin feature/minha-feature
```

---

# 📝 Licença

Este projeto está licenciado sob a licença MIT.

Veja o arquivo `LICENSE` para mais informações.

---

# 👨‍💻 Autor

Desenvolvido por **Fabricio Perrone**.

---

# ⭐ Considerações Finais

O MDSharp é um projeto avançado de emulação e análise do Mega Drive, focado em fidelidade técnica, estudo de hardware e ferramentas de debugging.

Se este projeto ajudou você ou foi útil para aprendizado, considere deixar uma ⭐ no repositório.
