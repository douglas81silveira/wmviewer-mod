# WMViewer – WhatsApp MsgStore Viewer (Modified Version)

WMViewer is a modified version of the **WhatsApp MsgStore Viewer** project, adapted to meet specific workflow and deployment needs.

This version focuses on:
- Distribution as a **single executable**
- Persistent local user data
- Improved file selection experience

---

## 🚀 Features

- 📦 **Single-file executable**
  - Packaged using **PyInstaller** with all required assets embedded.
- 💾 **Persistent login data**
  - Automatically creates and reads a `login_data.json` file in the **current directory**.
- 📂 **Improved file manager behavior**
  - `TextFieldFileManager` opens:
    - The **current directory** by default
    - Or **previously saved directories** from `login_data.json`, if available.
- 🖥️ **Windowed application**
  - No console window when running the executable.

---

## 🛠️ Build Command

```bash
pyinstaller --noconfirm --onefile --windowed --add-data "dbs;dbs" --add-data "View;View" --add-data "assets;assets" --add-data "about;." --add-data "LICENSE;." --add-data "credits;." --hidden-import "kivymd.uix.toolbar" --hidden-import "kivymd.uix.filemanager" --hidden-import "kivymd.uix.selectioncontrol" --name "WMViewer" --clean  "C:\Users\intel\whatsapp-msgstore-viewer\main.py"
```

---

## 📁 Runtime Files

- **`login_data.json`**
  - Created automatically in the directory where the executable is run.
  - Stores login information and previously accessed directories.
  - Reused on subsequent executions to improve usability.

---

## 📌 Notes

- This project is a **modified version**, not the original WhatsApp MsgStore Viewer.
- The original project credits and license are preserved.
- Designed for environments where portability and ease of deployment are required.

---

## 📄 License & Credits

Refer to the included `LICENSE` and `credits` files for original authorship and licensing information.

---

---

# WMViewer – WhatsApp MsgStore Viewer (Versão Modificada)

O **WMViewer** é uma versão modificada do projeto **WhatsApp MsgStore Viewer**, adaptada para atender demandas específicas de uso e distribuição.

Esta versão tem foco em:
- Distribuição como **executável único**
- Persistência de dados locais do usuário
- Melhor experiência na seleção de arquivos

---

## 🚀 Funcionalidades

- 📦 **Executável em arquivo único**
  - Empacotado com **PyInstaller**, incluindo todos os recursos necessários.
- 💾 **Dados de login persistentes**
  - Cria e lê automaticamente o arquivo `login_data.json` no **diretório atual**.
- 📂 **Comportamento aprimorado do gerenciador de arquivos**
  - O `TextFieldFileManager` abre:
    - O **diretório atual** por padrão
    - Ou **diretórios previamente salvos** no `login_data.json`, se existir.
- 🖥️ **Aplicação em modo janela**
  - Não abre console ao executar o programa.

---

## 🛠️ Comando de Build

```bash
pyinstaller --noconfirm --onefile --windowed --add-data "dbs;dbs" --add-data "View;View" --add-data "assets;assets" --add-data "about;." --add-data "LICENSE;." --add-data "credits;." --hidden-import "kivymd.uix.toolbar" --hidden-import "kivymd.uix.filemanager" --hidden-import "kivymd.uix.selectioncontrol" --name "WMViewer" --clean  "C:\Users\intel\whatsapp-msgstore-viewer\main.py"
```

---

## 📁 Arquivos em Tempo de Execução

- **`login_data.json`**
  - Criado automaticamente no diretório onde o executável é executado.
  - Armazena informações de login e diretórios acessados anteriormente.
  - Reutilizado nas próximas execuções para melhorar a usabilidade.

---

## 📌 Observações

- Este projeto é uma **versão modificada**, não o projeto original.
- Os créditos e a licença do projeto original foram mantidos.
- Desenvolvido para cenários que exigem portabilidade e facilidade de implantação.

---

## 📄 Licença e Créditos

Consulte os arquivos `LICENSE` e `credits` incluídos no projeto para informações sobre autoria e licenciamento original.
