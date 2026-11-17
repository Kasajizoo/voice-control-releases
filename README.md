# Voice Control — instalador Windows

Repositório público exclusivo para distribuição do **Voice Control**, protótipo acadêmico desenvolvido na Escola Politécnica da Universidade de São Paulo (Poli-USP), na disciplina PTC 3528 — Projeto de Formatura.

Este repositório **não contém o código-fonte do aplicativo**, modelos de desenvolvimento, dados experimentais ou arquivos privados. O instalador está disponível como anexo nas [GitHub Releases](https://github.com/Kasajizoo/voice-control-releases/releases).

## Versão de distribuição

- Voice Control **0.2.61** (W261)
- Windows 10 ou 11, 64 bits; microfone funcional
- Instalação local para o usuário atual
- Aproximadamente 81 MB para o instalador
- SHA-256 do arquivo `VoiceControl-Setup.exe`: `bd0bbca02b3acc19ef4c4b63eb1a99a8e31b2f1c507bad178e631db19215b058`

No PowerShell, é possível verificar o arquivo obtido:

```powershell
Get-FileHash -Algorithm SHA256 .\VoiceControl-Setup.exe
```

O Voice Control usa **VB-CABLE** para encaminhar o áudio tratado a outros aplicativos. Esse driver é fornecido separadamente pela VB-Audio: https://vb-audio.com/Cable/. Após instalar ou atualizar o driver, reinicie o Windows. O instalador do Voice Control **não instala nem altera drivers do sistema**.

O executável é uma compilação experimental de projeto acadêmico, sem assinatura digital de editor validada. O Windows poderá apresentar avisos de reputação ou segurança. Não desative o antivírus nem ignore alertas para executar o programa; verifique a procedência e integridade do arquivo.

## Apresentação e projeto

- [Vídeo de apresentação](https://youtu.be/4-QZL6hpJyg)
- [Estudo de caso e capturas reais da interface](https://qedxyzyt-dot.github.io/cases/?project=tcc)

## Componentes de terceiros

A aplicação utiliza componentes de processamento de áudio, bibliotecas Python/C++, Qt/PySide6 e runtimes de inferência. Cada componente mantém seus direitos e termos de licença; este repositório não transfere a propriedade ou a autoria desses componentes. O VB-CABLE é um produto da VB-Audio e não é distribuído pelo instalador do Voice Control.

## Equipe

Augusto Massayoshi Yojo de Lima · Gabriel Almeida Mathias · Lucas Galvão de França

Orientação: Prof. Dr. Juan Luis Poletti Soto · Escola Politécnica da USP · 2026.
