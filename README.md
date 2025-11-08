# Minhas Configurações do VSCode

Configurações personalizadas do Visual Studio Code com integração Vim e atalhos customizados.

## 📋 Recursos

- **Vim Integration**: Configuração completa do VSCodevim
  - ⚠️ **Requer extensão**: vscodevim.vim (v1.31.0+)
- **Leader Key**: Space como tecla leader
- **Navegação**: Atalhos Vim-like com Ctrl+hjkl
- **File Explorer**: Atalhos customizados para manipulação de arquivos
- **Temas**: Halcyon color theme

## ⚡ Setup Rápido

```bash
# 1. Instalar a extensão Vim (OBRIGATÓRIO)
code --install-extension vscodevim.vim

# 2. Clonar este repositório
git clone https://github.com/SEU-USUARIO/vscode-settings.git

# 3. Copiar configurações (escolha seu OS)
# Windows:
Copy-Item vscode-settings\*.json -Destination "$env:APPDATA\Code\User\" -Force

# Linux/Mac:
cp vscode-settings/*.json ~/.config/Code/User/

# 4. Reiniciar o VSCode
```

## 🚀 Instalação

### 1. Backup das Configurações Atuais (Opcional)

```bash
# Windows
cd %APPDATA%\Code\User
mkdir backup
copy settings.json backup\
copy keybindings.json backup\

# Linux/Mac
cd ~/.config/Code/User
mkdir backup
cp settings.json backup/
cp keybindings.json backup/
```

### 2. Clonar o Repositório

```bash
git clone https://github.com/SEU-USUARIO/vscode-settings.git
```

### 3. Copiar os Arquivos

**Windows (PowerShell):**
```powershell
Copy-Item vscode-settings\settings.json -Destination "$env:APPDATA\Code\User\" -Force
Copy-Item vscode-settings\keybindings.json -Destination "$env:APPDATA\Code\User\" -Force
```

**Linux/Mac:**
```bash
cp vscode-settings/settings.json ~/.config/Code/User/
cp vscode-settings/keybindings.json ~/.config/Code/User/
```

### 4. Instalar Extensões Necessárias

#### ⚠️ OBRIGATÓRIO

**Vim Extension** - Sem essa extensão, as configurações não funcionarão!

```
Name: Vim
Id: vscodevim.vim
Version: 1.31.0+
Publisher: vscodevim
```

**Instalação:**
- Via VSCode: `Ctrl+P` → `ext install vscodevim.vim`
- Via Terminal: `code --install-extension vscodevim.vim`
- [VS Marketplace](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)


## ⌨️ Atalhos Principais

### Leader Key Mappings (Space)

# Guia Completo de Atalhos - VSCode com Vim

## 🎯 Leader Key

A tecla **Leader** está configurada como **Space** (barra de espaço).

---

## 📁 Gerenciamento de Arquivos

### Salvar e Fechar

| Atalho | Ação | Modo |
|--------|------|------|
| `Space + w` | Salvar arquivo | Normal |
| `Space + x` | Salvar e fechar (`:x!`) | Normal |
| `Space + q` | Fechar sem salvar (`:q!`) | Normal |

### Splits (Divisão de Tela)

| Atalho | Ação | Modo |
|--------|------|------|
| `Space + sv` | Split vertical (`:vsplit`) | Normal |
| `Space + sh` | Split horizontal (`:split`) | Normal |

---

## 🔍 Busca e Navegação de Arquivos

| Atalho | Ação | Modo |
|--------|------|------|
| `Space + ff` | Quick open (buscar arquivo) | Normal |
| `Space + fs` | Find in files (buscar em arquivos) | Normal |
| `Space + nh` | Limpar highlight de busca (`:nohl`) | Normal |
| `Space + e` | Toggle sidebar (mostrar/ocultar explorer) | Normal |

---

## 🧭 Navegação Entre Painéis

### Movimento Entre Splits

| Atalho | Ação | Contexto |
|--------|------|----------|
| `Ctrl + h` | Navegar para esquerda | Editor |
| `Ctrl + l` | Navegar para direita | Editor + File Explorer |
| `Ctrl + j` | Navegar para baixo | Editor |
| `Ctrl + k` | Navegar para cima | Editor |

### Navegação Entre Abas/Buffers

| Atalho | Ação |
|--------|------|
| `Ctrl + [` | Editor anterior (aba à esquerda) |
| `Ctrl + ]` | Próximo editor (aba à direita) |

---

## 📂 File Explorer (Explorador de Arquivos)

**Contexto:** Quando o foco está no explorador de arquivos

| Atalho | Ação |
|--------|------|
| `a` | Criar novo arquivo |
| `Ctrl + n` | Criar nova pasta |
| `e` | Renomear arquivo/pasta |
| `d` | Deletar arquivo/pasta |
| `c` | Copiar |
| `Ctrl + p` | Colar |
| `Ctrl + x` | Cortar |
| `Ctrl + l` | Expandir/Entrar na pasta selecionada |

---

## 🔎 Quick Open (Busca Rápida)

**Contexto:** Quando a paleta Quick Open está aberta (`Space + ff` ou `Ctrl + p`)

| Atalho | Ação |
|--------|------|
| `Ctrl + j` | Selecionar próxima sugestão |
| `Ctrl + k` | Selecionar sugestão anterior |

---

## 💡 Autocomplete e Sugestões

**Contexto:** Quando o widget de sugestões está visível

| Atalho | Ação |
|--------|------|
| `Ctrl + j` | Próxima sugestão |
| `Ctrl + k` | Sugestão anterior |

---

## 🎯 Navegação de Código (Vim Mappings)

| Atalho | Ação | Modo |
|--------|------|------|
| `gi` | Go to implementation (ir para implementação) | Normal |
| `gr` | Show references (mostrar referências) | Normal |
| `K` | Show hover (mostrar documentação) | Normal |

---

## 🔧 Git

| Atalho | Ação | Modo |
|--------|------|------|
| `Space + hr` | Reverter mudanças selecionadas | Normal |

---

## ✏️ Edição em Modo Visual

| Atalho | Ação | Modo |
|--------|------|------|
| `<` | Diminuir indentação | Visual |
| `>` | Aumentar indentação | Visual |

---

## 🔄 Seleção Múltipla

| Atalho | Ação | Contexto |
|--------|------|----------|
| `Ctrl + n` | Adicionar seleção para próxima ocorrência | Editor (texto selecionado) |

---

## 🎛️ Painel e Terminal

| Atalho | Ação |
|--------|------|
| `Ctrl + .` | Toggle panel (mostrar/ocultar terminal/painel inferior) |

---

## 🔤 Recursos Vim Habilitados

- **Surround**: Adicionar/remover delimitadores ao redor de texto
- **EasyMotion**: Navegação rápida por caracteres visíveis
- **Incremental Search**: Busca incremental enquanto digita
- **Smart Relative Line**: Números de linha relativos inteligentes
- **System Clipboard**: Integração com clipboard do sistema

---

## 💾 Configurações Automáticas

- **Auto Save**: Salvamento automático após delay
- **Linked Editing**: Edição sincronizada de tags HTML
- **Search Highlight**: 
  - Cor de fundo: `#f6ff0080` (amarelo translúcido)
  - Cor do texto: `#fff` (branco)

---

## 🚫 Atalhos Desabilitados

Estes atalhos padrão do VSCode foram desabilitados para evitar conflitos:

| Atalho Original | Estava mapeado para |
|-----------------|---------------------|
| `Ctrl + o` | Open file |
| `Ctrl + n` | New untitled file |
| `Ctrl + h` | Find and Replace |
| `Ctrl + j` | Toggle panel |

---

## 📝 Notas

- **Leader Key Timeout**: Após pressionar Space, você tem um breve momento para pressionar a próxima tecla
- **Modo Insert vs Normal**: A maioria dos atalhos funcionam apenas em modo Normal
- **File Explorer Focus**: Os atalhos do explorer só funcionam quando o foco está nele (pressione `Space + e` para focar)

---

## 🎓 Dicas de Uso

1. **Buscar arquivos rapidamente**: `Space + ff` e comece a digitar o nome
2. **Navegar entre arquivos abertos**: Use `Ctrl + [` e `Ctrl + ]`
3. **Organizar janela**: `Space + sv` para split vertical, depois `Ctrl + h/l` para navegar
4. **Limpar busca**: Depois de buscar algo com `/`, use `Space + nh` para limpar o highlight
5. **Múltiplas seleções**: Selecione uma palavra, pressione `Ctrl + n` repetidamente para selecionar próximas ocorrências

---

**Última atualização**: Novembro 2025

## 🔧 Personalizações

Para ajustar as configurações ao seu gosto, edite os arquivos:

- **settings.json**: Configurações gerais e do Vim
- **keybindings.json**: Atalhos de teclado personalizados

## 📝 Notas

- Auto-save está habilitado com delay
- Linked editing está ativo
- Sistema de clipboard integrado com Vim
- Search highlight personalizado
- Smart relative line numbers

## 🤝 Contribuindo

Sinta-se à vontade para fazer fork deste repositório e adaptá-lo às suas necessidades!

## 📄 Licença

MIT License - Sinta-se livre para usar e modificar.

---

⭐ Se você achou útil, considere dar uma estrela no repositório!
