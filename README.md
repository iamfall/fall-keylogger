# fall-keylogger
Simple keylogger developed in C, using the Windows API.

-------------------------------------

Este projeto é um keylogger simples desenvolvido em C, utilizando a API do Windows. O objetivo é **educacional**, com foco em análise de segurança, engenharia reversa e testes de persistência. Não estou fazendo nada para ser usado na maldade.

> ⚠️ Uso permitido apenas em ambientes controlados e para fins educacionais.

## ✅ Funcionalidades

- Captura de teclas via `GetAsyncKeyState()`
- Persistência por Registro (`HKCU\Software\Microsoft\Windows\CurrentVersion\Run`)
- Oculta a janela no modo console
- Salva as teclas em `AppData\Roaming\log.txt`

## 🛠️ Compilação

Requer [MinGW](https://www.mingw-w64.org/) ou compilador compatível com WinAPI.

```bash
gcc keylogger.c -o fall_logger.exe -mwindows
