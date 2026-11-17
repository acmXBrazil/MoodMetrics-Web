# MOODMETRICS – Versão Web

Instrumento de Avaliação do Espectro do Humor (versão isolada para testes na web / WordPress).

## Arquivos essenciais

- `sci_moods_streamlit.py` — aplicação principal
- `textos_diagnosticos.json` — textos dos diagnósticos
- `Comorbidades/interferencias_template.md` — interferências / comorbidades
- `requirements.txt` — dependências Python

## Como rodar localmente

```bash
pip install -r requirements.txt
streamlit run sci_moods_streamlit.py
```

## Como colocar no WordPress

A forma mais simples e segura é:

1. Hospedar este app no **Streamlit Community Cloud** (grátis):
   - Crie um repositório no GitHub com esta pasta.
   - Acesse https://share.streamlit.io e faça o deploy.

2. No WordPress, embede via iframe:

```html
<iframe 
  src="https://seu-app.streamlit.app" 
  width="100%" 
  height="800" 
  frameborder="0" 
  style="border: none; border-radius: 8px;">
</iframe>
```

> Observação: o Streamlit Community Cloud tem limites de uso gratuito. Para produção maior, considere Streamlit em servidor próprio ou alternativas.

## Citações (bibliografia)

A pasta `citacoes/` é opcional. Se quiser exibir bibliografia no relatório, coloque os arquivos `.txt` (01.txt, 02.txt...) dentro dela.

## Isolamento

Esta pasta é uma cópia isolada do projeto original. Alterações aqui não afetam o `Projeto_questionario` original.
