# Península · Vila Madalena

Landing page de captação de leads para o empreendimento **Península**, localizado na Vila Madalena, São Paulo.

## 🚀 Deploy

Hospedado via **GitHub Pages**. Acesse em:
```
https://<seu-usuario>.github.io/<nome-do-repo>/
```

## 📋 Sobre

Single page de alta conversão com formulário multistep (3 etapas) integrado ao Google Sheets via Apps Script.

**Tipologias apresentadas:**
- 154m² · 3 suítes · 2 vagas
- 193m² · 4 suítes · 3 vagas
- Cobertura 300m² · exclusiva

## ⚙️ Integração Google Sheets

Os leads são enviados automaticamente para a planilha via Google Apps Script.

**Para trocar a planilha de destino:**

1. Abra o arquivo `index.html`
2. Localize a variável `SHEETS_URL` no final do arquivo
3. Substitua pela URL do seu novo Apps Script

```js
var SHEETS_URL = 'https://script.google.com/macros/s/SEU_SCRIPT_ID/exec';
```

**Campos capturados:**
| Campo | Descrição |
|-------|-----------|
| Data | Data e hora do envio |
| Nome | Nome completo |
| WhatsApp | Telefone formatado |
| Email | E-mail |
| Interesse | Tipologia selecionada |
| Projeto | Identificador do projeto |

## 📁 Estrutura

```
/
├── index.html       # Landing page completa (HTML + CSS + JS inline)
└── README.md
```

> Tudo em um único arquivo para facilitar o deploy no GitHub Pages.

## 🌐 Como publicar no GitHub Pages

1. Renomeie `peninsula_v3.html` para `index.html`
2. Crie um repositório no GitHub
3. Faça o push dos arquivos
4. Vá em **Settings → Pages**
5. Source: **Deploy from a branch → main → / (root)**
6. Aguarde ~1 minuto e o link estará ativo

## 🛠️ Tecnologias

- HTML5 / CSS3 / JavaScript vanilla
- Google Fonts (Cormorant Garamond + Montserrat)
- Google Apps Script (backend do formulário)
