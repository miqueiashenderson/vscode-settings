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

| Atalho | Ação |
|--------|------|
| `Space + w` | Salvar arquivo |
| `Space + x` | Salvar e fechar |
| `Space + q` | Fechar sem salvar |
| `Space + sv` | Split vertical |
| `Space + sh` | Split horizontal |
| `Space + e` | Toggle sidebar |
| `Space + ff` | Quick open (buscar arquivo) |
| `Space + fs` | Find in files |
| `Space + nh` | No highlight (limpar busca) |

### Vim Mappings

| Atalho | Ação |
|--------|------|
| `gi` | Go to implementation |
| `gr` | Show references |
| `K` | Show hover |

### Navegação Entre Painéis

| Atalho | Ação |
|--------|------|
| `Ctrl + h` | Navegar para esquerda |
| `Ctrl + l` | Navegar para direita |
| `Ctrl + j` | Navegar para baixo |
| `Ctrl + k` | Navegar para cima |
| `Ctrl + [` | Editor anterior |
| `Ctrl + ]` | Próximo editor |

### File Explorer

| Atalho | Ação |
|--------|------|
| `a` | Novo arquivo |
| `Ctrl + n` | Nova pasta |
| `e` | Renomear |
| `d` | Deletar |
| `c` | Copiar |
| `Ctrl + p` | Colar |
| `Ctrl + x` | Cortar |

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
