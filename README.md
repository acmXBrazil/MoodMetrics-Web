# MOODMETRICS – Versão Web

Instrumento de Avaliação do Espectro do Humor  
Versão isolada para testes na web / WordPress.

## Estrutura

```
MoodMetrics_Web/
├── Comorbidades/
│   └── interferencias_template.md
├── citacoes/                  ← arquivos .txt da bibliografia (01.txt, 02.txt...)
├── sci_moods_streamlit.py     ← aplicação principal
├── textos_diagnosticos.json
├── requirements.txt
├── .gitignore
└── README.md
```

## Como rodar localmente

```bash
pip install -r requirements.txt
streamlit run sci_moods_streamlit.py
```

## Deploy no Streamlit Community Cloud

1. Crie um repositório **público** no GitHub com o conteúdo desta pasta.
2. Acesse [share.streamlit.io](https://share.streamlit.io) e faça login com o GitHub.
3. Clique em **New app**.
4. Selecione o repositório.
5. Main file path: `sci_moods_streamlit.py`
6. Clique em **Deploy**.

## Embutir no WordPress

Depois do deploy, use um bloco HTML no WordPress:

```html
<iframe 
  src="https://SEU-APP.streamlit.app" 
  width="100%" 
  height="850" 
  frameborder="0" 
  style="border:none; border-radius:8px;">
</iframe>
```

Substitua `https://SEU-APP.streamlit.app` pela URL real gerada pelo Streamlit Cloud.

## Observações

- A pasta `citacoes/` deve ser enviada para o repositório para a bibliografia aparecer no PDF.
- Dados demográficos são coletados de forma anônima no início.
- Esta versão é isolada do projeto original.
