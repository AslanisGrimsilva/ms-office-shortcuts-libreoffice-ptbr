# Guia Rápido de Instalação

Este guia cobre apenas o essencial para instalar os atalhos. Para informações completas sobre o projeto, limitações e atalhos mapeados, consulte o [README completo](README.md).

---

## 1. Faça backup da sua configuração atual

Antes de qualquer coisa, salve os atalhos atuais do LibreOffice para poder restaurá-los se precisar.

1. Abra o LibreOffice Writer (ou Calc, ou Impress) com um documento em branco.
2. Vá em **Ferramentas > Personalizar > aba Teclado**.
3. Clique em **Salvar...** e salve em algum lugar seguro com um nome como `backup_writer.cfg`.
4. Repita para Calc e Impress.

---

## 2. Baixe os arquivos

Na pasta `dist/` deste repositório, baixe o(s) arquivo(s) que você precisa:

| Arquivo | Programa |
|---|---|
| `Word_Shortcuts_para_Writer_PTBR_v3.cfg` | LibreOffice Writer |
| `Excel_Shortcuts_para_Calc_PTBR_v3.cfg` | LibreOffice Calc |
| `PowerPoint_Shortcuts_para_Impress_PTBR_v2.cfg` | LibreOffice Impress |

Para baixar: clique no arquivo, depois em **Download raw file** (ícone de download no canto superior direito do conteúdo).

---

## 3. Instale

Repita os passos abaixo para cada programa que quiser configurar:

1. Abra o LibreOffice Writer, Calc ou Impress com um documento aberto.
2. Vá em **Ferramentas > Personalizar > aba Teclado**.
3. Clique em **Carregar...** e selecione o arquivo `.cfg` correspondente.
4. Clique em **OK**.

Pronto. Os atalhos do Office PT-BR estão ativos.

---

## Limitações principais

- **Ctrl+Shift+^** (formato científico no Calc): não funciona no LibreOffice em nenhum sistema operacional.
- **Linux com GNOME** (Zorin OS, Ubuntu, Fedora etc.): o atalho **Ctrl+Alt+D** (Nota de fim no Writer) é capturado pelo sistema para mostrar a área de trabalho. O Super+D faz a mesma função, então desativar o Ctrl+Alt+D do sistema não implica perda de funcionalidade. Veja o README completo para instruções.
