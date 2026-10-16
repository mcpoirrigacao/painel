# Painel da Diretoria — MCPO / MAQCAMPO

Painel **somente leitura** que reúne os indicadores dos apps internos:
CRM Comercial, Faturamento, Assistência Técnica, Obras de Montagem e Orçamentos.

**Acesso:** https://mcpoirrigacao.github.io/painel/

- Login com a conta Microsoft da MAQCAMPO (pede só permissão de leitura).
- Lê os mesmos arquivos que os apps usam no SharePoint MCPOIRRIGACAO e a planilha do CRM pelo Apps Script.
- Não grava nada: toda chamada de rede passa por uma função que recusa qualquer método diferente de GET.
- Entra quem é administrador em algum dos apps, ou quem estiver em `Painel Diretoria/painel_acesso.json` no SharePoint.
- Nenhuma senha e nenhum dado ficam neste repositório. A senha da planilha do CRM é digitada na aba ⚙ Fontes e fica só no navegador.
