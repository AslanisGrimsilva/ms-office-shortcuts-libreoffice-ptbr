# Atalhos do Microsoft Office (PT-BR) para o LibreOffice

Este repositório fornece arquivos de configuração prontos para o LibreOffice que substituem os atalhos de teclado padrão pelos atalhos do Microsoft Office **em português do Brasil** — os mesmos que aparecem nos menus do Word, Excel e PowerPoint quando o sistema está em português.

Os arquivos foram testados no **LibreOffice para Windows** e no **Zorin OS 18** (Linux, teclado ABNT2).

> **Atenção:** Este projeto é um fork de [Zaki101Aslam/MS-office-shortcuts-for-Libre-Office](https://github.com/Zaki101Aslam/MS-office-shortcuts-for-Libre-Office), publicado sob a licença [Mozilla Public License 2.0](LICENSE). Os arquivos `.cfg` gerados aqui são derivados desse trabalho e estão sujeitos à mesma licença.

---

## Por que este fork existe?

O projeto original mapeia os atalhos do Office em **inglês** (por exemplo, Ctrl+G = "Go To", Ctrl+F = "Find"). No Office instalado em **português do Brasil**, muitos atalhos são diferentes: Ctrl+G = Alinhar à direita, Ctrl+L = Localizar, Ctrl+B = Salvar, e assim por diante.

Este fork adapta os mapeamentos para o português do Brasil, com base em fontes primárias (lista exportada do próprio Word via macro `Application.ListCommands`) e em testes diretos no Excel e no PowerPoint.

---

## Arquivos disponíveis

Na pasta `dist/` você encontra três arquivos prontos para uso:

| Arquivo | Para usar no | Equivalente ao |
|---|---|---|
| `Word_Shortcuts_para_Writer_PTBR_v3.cfg` | LibreOffice Writer | Microsoft Word PT-BR |
| `Excel_Shortcuts_para_Calc_PTBR_v3.cfg` | LibreOffice Calc | Microsoft Excel PT-BR |
| `PowerPoint_Shortcuts_para_Impress_PTBR_v2.cfg` | LibreOffice Impress | Microsoft PowerPoint PT-BR |

---

## Como instalar

> **Antes de começar: faça um backup da sua configuração atual.**
> Veja a seção [Fazendo backup antes de instalar](#fazendo-backup-antes-de-instalar) abaixo.

### Passo a passo (igual para Writer, Calc e Impress)

1. Baixe o arquivo `.cfg` correspondente ao programa que você quer configurar.  
   *(Clique no arquivo na pasta `dist/`, depois clique em "Download raw file" ou no ícone de download.)*

2. Abra o LibreOffice Writer, Calc ou Impress — **com um documento aberto** (pode ser um documento em branco).

3. No menu superior, clique em **Ferramentas**.

4. Clique em **Personalizar...** (pode aparecer como "Personalizar" ou "Personalizar teclado").

5. Na janela que abrir, clique na aba **Teclado**.

6. No lado direito da janela, clique no botão **Carregar...** (em algumas versões aparece como "Load...").

7. Navegue até a pasta onde você salvou o arquivo `.cfg` e selecione-o.

8. Clique em **Abrir**.

9. Clique em **OK** para fechar a janela de personalização.

10. Pronto! Os atalhos do Office PT-BR agora estão ativos naquele programa.

> **Repita os passos 2 a 10** para cada programa (Writer, Calc, Impress), usando o `.cfg` correspondente.

---

## Fazendo backup antes de instalar

Antes de carregar qualquer `.cfg`, salve a configuração atual do LibreOffice. Assim você pode voltar atrás se quiser.

### No LibreOffice Writer (ou Calc, ou Impress)

1. Abra o programa com um documento em branco.
2. Vá em **Ferramentas > Personalizar... > aba Teclado**.
3. Clique no botão **Salvar...** (ou "Save...") — **não confunda com "Carregar"**.
4. Escolha uma pasta fácil de encontrar (por exemplo, sua pasta Documentos) e salve com um nome como `backup_writer_original.cfg`.
5. Repita para Calc e Impress.

Esses arquivos de backup podem ser carregados da mesma forma para restaurar os atalhos originais.

---

## O que foi mapeado

### Writer (baseado no Word PT-BR)

A tabela abaixo lista os principais atalhos configurados. A coluna **Status** indica se o atalho foi confirmado diretamente no Word, inferido por comparação com outras fontes, ou ainda precisa de teste.

| Ação | Atalho PT-BR | Status |
|---|---|---|
| Salvar | Ctrl+B | ✅ Confirmado |
| Negrito | Ctrl+N | ✅ Confirmado |
| Itálico | Ctrl+I | ✅ Confirmado |
| Sublinhado | Ctrl+S | ✅ Confirmado |
| Selecionar tudo | Ctrl+T | ✅ Confirmado |
| Localizar | Ctrl+L | ✅ Confirmado |
| Substituir | Ctrl+U | ✅ Confirmado |
| Refazer | Ctrl+R | ✅ Confirmado |
| Ir para | Ctrl+Alt+G | ✅ Confirmado |
| Copiar formato | Ctrl+Alt+C | ✅ Confirmado |
| Colar somente texto | Ctrl+Shift+V | ✅ Confirmado |
| Subscrito | Ctrl+Shift+- | ✅ Confirmado |
| Recuo deslocado | Ctrl+H | ✅ Confirmado |
| Estilo Normal | Ctrl+Shift+Y | ✅ Confirmado |
| Inserir comentário | Ctrl+Alt+A | ✅ Confirmado |
| Nota de fim | Ctrl+Alt+D | ✅ Confirmado |
| Alinhar à esquerda | Ctrl+Q | ✅ Confirmado |
| Alinhar à direita | Ctrl+G | ✅ Confirmado |
| Centralizar | Ctrl+E | ✅ Confirmado |
| Justificar | Ctrl+J | ✅ Confirmado |
| Título 1 | Ctrl+Shift+1 | ⚠️ Inferido |
| Título 2 | Ctrl+Shift+2 | ⚠️ Inferido |
| Título 3 | Ctrl+Shift+3 | ⚠️ Inferido |
| Novo documento | Ctrl+O | ✅ Confirmado |
| Fechar | Ctrl+W | ✅ Confirmado |

> **Atalhos sem equivalente no LibreOffice e descartados:** comandos do Copilot, marcas XML, painéis do Office 365 e funções exclusivas da faixa de opções sem atalho funcional equivalente.

### Calc (baseado no Excel PT-BR)

| Ação | Atalho PT-BR | Status |
|---|---|---|
| Abrir | Ctrl+A | ✅ Confirmado |
| Selecionar tudo | Ctrl+T | ✅ Confirmado |
| Preencher à direita | Ctrl+R | ✅ Confirmado |
| Preencher acima | Ctrl+H | ✅ Confirmado |
| Refazer | Ctrl+Y | ✅ Confirmado |
| Localizar e Substituir | Ctrl+L | ✅ Confirmado |
| Filtro Automático | Ctrl+Shift+L | ✅ Confirmado |
| Formato moeda ($) | Ctrl+Shift+4 | ✅ Confirmado |
| Formato percentual (%) | Ctrl+Shift+5 | ✅ Confirmado |
| Formato científico | Ctrl+Shift+^ | ❌ Não funciona no LibreOffice |
| Formato de data | Ctrl+Shift+3 | ✅ Confirmado |
| Inserir hora | Ctrl+Alt+Q | ✅ Confirmado |
| Formato número (decimal) | Ctrl+Shift+1 | ✅ Confirmado |

> **Atenção — Ctrl+Shift+^ (formato científico):** Este atalho **não funciona no LibreOffice Calc**, nem no Windows nem no Linux. O LibreOffice não consegue capturar essa combinação com o `^` do teclado ABNT2. O atalho foi mantido na tabela apenas para documentar a diferença em relação ao Excel. Se você precisar aplicar formato científico no Calc, use o menu **Formatar > Células > aba Números**.

### Impress (baseado no PowerPoint PT-BR)

| Ação | Atalho PT-BR | Status |
|---|---|---|
| Negrito | Ctrl+N | ✅ Confirmado |
| Salvar | Ctrl+B | ✅ Confirmado |
| Fechar | Ctrl+W | ✅ Confirmado |
| Refazer | Ctrl+Y | ✅ Confirmado |
| Alinhar à direita | Ctrl+R | ✅ Confirmado |
| Alinhar à esquerda | Ctrl+Q | ✅ Confirmado |
| Localizar e Substituir | Ctrl+L / Ctrl+U | ✅ Confirmado |
| Subscrito | Ctrl+= | ✅ Confirmado |
| Inserir comentário | Ctrl+Alt+M | ✅ Confirmado |
| Salvar como | Ctrl+Shift+S | ✅ Confirmado |
| Centralizar | Ctrl+Shift+E | ✅ Confirmado |

---

## Diferenças em relação ao projeto original

| Aspecto | Projeto original | Este fork |
|---|---|---|
| Idioma dos atalhos | Inglês (ex.: Ctrl+F = Localizar) | Português do Brasil (ex.: Ctrl+L = Localizar) |
| Fonte dos atalhos | Página de suporte da Microsoft em inglês | Lista exportada do próprio Office PT-BR + testes diretos |
| Público-alvo | Usuários com Office em inglês | Usuários com Office instalado em português do Brasil |
| Scripts Python | Mantidos sem alteração | Mantidos sem alteração (podem ser usados para gerar novos `.cfg`) |

---

## Limitações conhecidas

### Independente do sistema operacional

- O atalho Ctrl+Shift+^ (formato científico do Excel) **não funciona no LibreOffice Calc em nenhum sistema operacional** — o LibreOffice não consegue capturar essa combinação com o `^` do teclado ABNT2. Para aplicar formato científico no Calc, use o menu **Formatar > Células > aba Números**.
- Atalhos marcados como "Inferido" nas tabelas acima precisam de confirmação direta no Word/Excel/PowerPoint.
- Atalhos que dependem da faixa de opções do Office (Alt+letra) não foram mapeados, pois o LibreOffice usa uma estrutura diferente.

### No Linux — conflitos com atalhos do sistema

Alguns ambientes de desktop Linux reservam certas combinações de teclas para funções do sistema, e elas são capturadas **antes** de chegarem ao LibreOffice. O atalho do sistema prevalece, e o atalho do LibreOffice simplesmente não é executado.

Conflito confirmado no **Zorin OS 18** (ambiente GNOME):

| Atalho | Função no `.cfg` do Writer | Função no sistema (GNOME) |
|---|---|---|
| Ctrl+Alt+D | Nota de fim | Minimizar todas as janelas / mostrar área de trabalho |

Outros ambientes de desktop baseados em GNOME (Ubuntu, Fedora, Pop!_OS etc.) provavelmente apresentam o mesmo conflito com Ctrl+Alt+D, pois esse é o atalho padrão do GNOME para mostrar a área de trabalho. Distribuições com outros ambientes (KDE, XFCE, Cinnamon) podem ter conflitos diferentes ou nenhum conflito.

Vale notar que o GNOME oferece **dois atalhos** para a mesma função de mostrar a área de trabalho: Ctrl+Alt+D e Super+D (a tecla Super é a tecla Windows do teclado). Portanto, desativar o Ctrl+Alt+D do sistema **não perde a funcionalidade** — o Super+D continua funcionando normalmente.

**Como resolver**, se quiser:
- **Opção A — Desativar apenas o Ctrl+Alt+D do sistema (recomendada):** vá em Configurações > Teclado > Atalhos de teclado > Navegação, encontre "Mostrar área de trabalho" ou "Ocultar todas as janelas normais", clique nele e pressione Backspace para remover a atribuição. O Super+D continuará funcionando para mostrar a área de trabalho.
- **Opção B — Remover o atalho do LibreOffice:** abra o Writer, vá em Ferramentas > Personalizar > Teclado, encontre o atalho Ctrl+Alt+D e clique em "Excluir". O Ctrl+Alt+D do sistema voltará a funcionar normalmente.

As duas opções são independentes — escolha a que fizer mais sentido para o seu uso.

---

## Como usar os scripts Python para gerar seus próprios arquivos

Os scripts originais do projeto (`src/generate_config.py`) continuam funcionando. Você pode usá-los para personalizar os mapeamentos:

1. Edite os arquivos JSON em `mappings/` (um para cada programa).
2. Execute o script para gerar um novo `.cfg`:
   ```bash
   python3 src/generate_config.py
   ```
3. Os arquivos gerados aparecerão na pasta `dist/`.

Para mais detalhes, consulte o README do projeto original (em inglês).

---

## Créditos e licença

- **Projeto original:** [Zaki101Aslam/MS-office-shortcuts-for-Libre-Office](https://github.com/Zaki101Aslam/MS-office-shortcuts-for-Libre-Office)
- **Adaptação PT-BR:** [AslanisGrimsilva/ms-office-shortcuts-libreoffice-ptbr](https://github.com/AslanisGrimsilva/ms-office-shortcuts-libreoffice-ptbr)
- **Licença:** [Mozilla Public License 2.0](LICENSE) — o código-fonte e os arquivos de configuração derivados do projeto original estão sujeitos a esta licença.

A MPL-2.0 permite usar, modificar e redistribuir este trabalho, inclusive em projetos proprietários, desde que as modificações nos arquivos cobertos pela licença sejam disponibilizadas sob a mesma MPL-2.0. Você não precisa licenciar seu projeto inteiro sob a MPL-2.0, apenas os arquivos que vieram ou foram modificados a partir deste repositório.
