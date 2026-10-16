# Painel da Diretoria — MCPO / MAQCAMPO

**Acesso:** https://mcpoirrigacao.github.io/painel/

Reúne, em modo **visualização**, as telas dos apps internos: CRM Comercial, CRM SAM, Faturamento,
Assistência Técnica, Obras de Montagem e Orçamentos, mais uma Visão Geral resumida do mês.

## Como funciona
- Login com a conta Microsoft da MAQCAMPO.
- O painel lê os mesmos arquivos que os apps usam no SharePoint MCPOIRRIGACAO e a planilha do CRM (Apps Script).
- Cada área mostra **a própria tela do app** (o index.html publicado de cada repositório), aberta num quadro isolado:
  sem acesso à rede (não consegue gravar nada), sem login do app, com botões de cadastro/edição e a aba Parâmetros ocultos.
  O cabeçalho de cada app é escondido: as páginas dele viram o **submenu** do painel (e a data de referência, quando existe, fica no submenu).
  Melhorias publicadas nos apps aparecem aqui automaticamente.
- O CRM SAM lê a pasta "CRM SAM" do SharePoint; a tela dele conversa com um SharePoint simulado que só responde leitura.
- Orçamentos tem tela própria (o app de orçamentação não tem painel), com filtro de período e busca.

## Acesso e parâmetros
- Pasta **Painel** no SharePoint MCPOIRRIGACAO: `painel_acesso.json` (administradores e usuários comuns) e
  `painel_parametros.json` (áreas visíveis para comuns, atualização automática, modo TV, senha de leitura do CRM).
- É o único lugar onde o painel grava, pela aba **⚙ Fontes e Parâmetros**, visível só para administradores.
- Enquanto não houver administrador cadastrado, quem é administrador em algum dos apps entra como admin para fazer o primeiro cadastro.
- Nenhuma senha e nenhum dado ficam neste repositório.
