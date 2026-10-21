# SQL Toolkit (By Emerson Carlos)

🇧🇷 Português · [🇺🇸 English below](#-english)

Kit de ferramentas para SQL Server em **uma única página HTML**. Roda 100% no navegador: **nada é enviado e nada é guardado**.

🔗 **Usar online:** https://emersonsamuel.github.io/sql-toolkit/

## Ferramentas

| Ferramenta | O que faz |
|---|---|
| **Formatador SQL** | Organiza T-SQL com várias opções: caixa das palavras-chave, indentação (Tab/espaços), vírgula no fim ou no começo, CASE, IN, BETWEEN, JOIN/ON, quebras de linha, minificar e colorir. |
| **Desparametrizador** | Transforma `sp_executesql` em query com `DECLARE`, pronta para rodar. |
| **Anonimizador** | Troca nomes de objetos e valores antes de você compartilhar uma query. |
| **Analisador IO / TIME** | Lê a saída de `SET STATISTICS IO, TIME ON` e mostra totais e peso por tabela. |
| **Plano de execução** | Lê um `.sqlplan` (arquivo ou XML colado): alertas, índices ausentes e operadores ordenados por custo. |
| **Deadlock** | Lê o XML do deadlock e explica vítima, objetos e o motivo do impasse. |
| **Comparativo antes/depois** | Compara tempo, CPU e leituras antes e depois do tuning. |

## Como usar

- **Online:** abra o link acima.
- **Offline:** baixe o arquivo [`index.html`](index.html) (botão *Download raw file*) e abra no navegador. Não precisa de internet nem de instalação.

## Privacidade

A página não faz nenhuma requisição de rede (a política de segurança do próprio HTML bloqueia conexões externas) e não usa armazenamento. Ao fechar ou recarregar, o que você colou some.

## Limitações

- O analisador de IO/TIME lê a saída do SSMS **em inglês**.
- Os custos do plano de execução são estimativas do otimizador.
- É uma versão inicial. Se encontrar uma query que formata mal ou um XML que não é lido, abra uma *issue* — **sem dados reais ou confidenciais**: use um exemplo anonimizado.
- Confira sempre o resultado antes de usar em produção.

## Licença e autoria

Criado por **Emerson Carlos**. Licença [MIT](LICENSE): você pode usar, copiar e modificar, desde que mantenha o aviso de copyright e a licença.

---

## 🇺🇸 English

A SQL Server toolkit in **a single HTML page**. It runs 100% in your browser: **nothing is sent and nothing is stored**.

🔗 **Use it online:** https://emersonsamuel.github.io/sql-toolkit/

### Tools

| Tool | What it does |
|---|---|
| **SQL Formatter** | Formats T-SQL with many options: keyword case, indentation (tab/spaces), leading or trailing commas, CASE, IN, BETWEEN, JOIN/ON, line breaks, minify and syntax coloring. |
| **Deparameterizer** | Turns `sp_executesql` calls into a runnable query with `DECLARE`s. |
| **Anonymizer** | Replaces object names and values before you share a query. |
| **IO / TIME Analyzer** | Parses `SET STATISTICS IO, TIME ON` output and shows totals and per-table weight. |
| **Execution plan** | Reads a `.sqlplan` (file or pasted XML): warnings, missing indexes and operators sorted by cost. |
| **Deadlock** | Reads the deadlock XML and explains the victim, the objects and why it happened. |
| **Before/after comparison** | Compares duration, CPU and reads before and after tuning. |

### How to use

- **Online:** open the link above.
- **Offline:** download [`index.html`](index.html) (*Download raw file*) and open it in your browser. No internet or installation needed.

### Privacy

The page makes no network requests (the page's own security policy blocks outbound connections) and uses no storage. Close or reload and what you pasted is gone.

### Limitations

- The IO/TIME analyzer reads **English** SSMS output.
- Execution plan costs are optimizer estimates.
- This is an early version. If a query formats badly or an XML isn't read, open an issue — **without real or confidential data**: use an anonymized example.
- Always review the output before using it in production.

### License and authorship

Created by **Emerson Carlos**. [MIT](LICENSE) license: you may use, copy and modify it as long as you keep the copyright notice and the license.
