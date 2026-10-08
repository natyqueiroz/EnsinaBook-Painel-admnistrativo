# Painel Administrativo para Venda de Cursos

Sistema web de gestão para uma empresa que vende cursos com equipe de vendedores em campo: vendas, comissões, cancelamentos, eventos e renovações de contrato em um só lugar.

> 🧪 **Esta é a versão de demonstração.** Todos os dados são fictícios e ficam apenas na memória do navegador (recarregar a página reinicia tudo). Nenhuma informação é enviada a servidor algum.

**🔗 Demo online:** `COLE-AQUI-O-LINK-DO-GITHUB-PAGES`
**🔑 Login de visitante:** usuário `demo` · senha `demo`

## O que o sistema faz

- **Vendas:** cadastro com dados do cliente, brindes, duração do contrato, anexo da venda, busca e alerta de contrato duplicado.
- **Relatório de comissão:** cálculo por vendedor (valor com e sem brinde, vale, estornos) e exportação em PDF.
- **Controle de Cancelamento:** duas tabelas (análise/negociação e setor financeiro), prazo em dias úteis com contagem regressiva, alerta de análise atrasada, cálculo de multa (mais de 7 dias após a compra), Reclame Aqui e anexo da carta acordo.
- **Cancelados:** histórico permanente com comprovante de estorno.
- **Eventos:** datas, confirmados, custo, contrato e proposta anexados, e gráfico de desempenho (receita das vendas × custo).
- **Renovações:** lista de contratos vencidos ou a vencer.
- **Dashboard:** resumo, gráfico de vendas por mês e calendário da semana.
- **Controle de acesso:** perfis de administrador e funcionário, com telas diferentes para cada um.

## Tecnologias

- **Front-end:** HTML semântico, CSS (Flexbox/Grid, responsivo) e JavaScript puro, sem framework. Chart.js para gráficos e jsPDF para os PDFs.
- **Back-end da versão real:** Node.js, Express, SQLite (better-sqlite3), autenticação com JWT e bcrypt, upload de arquivos com multer, publicado em um VPS com PM2.
- **Nesta demo:** o servidor é substituído por uma API simulada dentro do próprio `index.html` (intercepta as chamadas `fetch('/api/...')`), o que permite publicar no GitHub Pages.

## Como rodar

Basta abrir o `index.html` no navegador, ou publicar no GitHub Pages:

1. Envie o `index.html` e este `README.md` para um repositório.
2. Em **Settings → Pages**, escolha a branch `main` (pasta `/root`) e salve.

## Autoria

Desenvolvido por **Nathaly Barbosa**.
