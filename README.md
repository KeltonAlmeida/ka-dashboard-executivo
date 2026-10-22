# KA • Dashboard Executivo de Orçamento

Dashboard responsivo para o portfólio de **Kelton Almeida (KA)**, com custos orçados e realizados, desvios por mês e por categoria, indicadores de desempenho e filtros dinâmicos.

> **Atenção: demonstração pública com dados 100% fictícios.** Não contém a planilha original, nem valores reais, informações pessoais, fornecedores ou registros de transações. Não utilize o HTML público como armazenamento de dados sigilosos.

## Recursos

- Indicadores orçados, realizados, desvios absolutos e percentuais.
- Gráficos mensais, distribuição das despesas e ranking de desvios.
- Filtros por mês, centro de custo e categoria.
- Alternância entre temas **claro e escuro**.
- Exportação CSV do resumo filtrado e impressão.
- Layout responsivo sem dependências externas, cookies ou analytics.

## Executar localmente

Abra `index.html` diretamente no navegador ou rode:

```bash
python -m http.server 8000
```

Acesse `http://localhost:8000`.

## Publicar no GitHub

1. Crie um repositório público chamado `ka-dashboard-executivo` em https://github.com/new (não marque README, pois este projeto já inclui um).
2. Extraia o ZIP e, pelo GitHub, use **Add file → Upload files** para enviar `index.html`, `styles.css`, `app.js`, `vercel.json`, `README.md` e `.gitignore` à raiz do repositório.
3. Faça o commit na branch `main`.

Alternativa pelo terminal na pasta extraída:

```bash
git init
git add .
git commit -m "feat: dashboard executivo KA com dados demonstrativos"
git branch -M main
git remote add origin https://github.com/KeltonAlmeida/ka-dashboard-executivo.git
git push -u origin main
```

## Publicar no Vercel

1. Entre em https://vercel.com/new e conecte sua conta GitHub.
2. Selecione `KeltonAlmeida/ka-dashboard-executivo`.
3. Configure o preset **Other**, **Root Directory:** `./`, sem build command e sem output directory customizado.
4. Clique em **Deploy**. O Vercel servirá o `index.html` da raiz.

Depois, commits na branch principal podem disparar novos deploys conforme a configuração do projeto.

## Estrutura

```text
ka-dashboard-executivo/
├── index.html       # Layout e componentes
├── styles.css       # Layout responsivo e temas
├── app.js           # Dados fictícios, filtros, indicadores, gráficos
├── vercel.json      # Cabeçalhos básicos de segurança
├── .gitignore       # Bloqueio de arquivos de dados originais
└── README.md        # Documentação
```

## Dados e privacidade

Os valores de `app.js` foram criados artificialmente para fins de portfólio, sem reutilizar os valores da planilha de referência. Dados inseridos em arquivos públicos do frontend são sempre acessíveis a qualquer visitante. Para uma versão real, utilize backend com autenticação, permissões e controles de acesso adequados, além de políticas de tratamento e retenção alinhadas à LGPD.

**Autor:** Kelton Almeida (KA).
