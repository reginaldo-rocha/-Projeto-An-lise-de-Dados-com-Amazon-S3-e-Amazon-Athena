# -Projeto-An-lise-de-Dados-com-Amazon-S3-e-Amazon-Athena

## 📌 Descrição
Este projeto demonstra a criação de um fluxo simples de análise de dados na AWS utilizando Amazon S3 e Amazon Athena, permitindo consultas SQL diretamente sobre arquivos armazenados na nuvem, sem necessidade de infraestrutura.

<img width="1536" height="1024" alt="imagem projeto hoje" src="https://github.com/user-attachments/assets/6b149a3b-bd6f-4f66-a738-b10665e6e760" />


## 🧱 Arquitetura do Projeto

Fluxo:
1. Upload de arquivo CSV no Amazon S3
2. Armazenamento dos dados na camada "dados/"
3. Criação de tabela externa no Amazon Athena
4. Execução de consultas SQL
5. (Opcional) Armazenamento dos resultados no S3
6. Visualização dos dados (Excel / Power BI / etc.)

---

## 🛠️ Tecnologias Utilizadas

- Amazon S3
- Amazon Athena
- SQL

---

## 📊 Exemplo de Consulta

```sql
SELECT 
  produto,
  SUM(valor) as total
FROM vendas
GROUP BY produto
ORDER BY total DESC;

💡 Benefícios da Arquitetura
Armazenamento escalável e seguro
Consultas SQL sem necessidade de servidores
Baixo custo (pay-per-query)
Implementação rápida
Ideal para análise exploratória de dados

📸 Evidências

Upload no S3
<img width="1359" height="675" alt="bucket scv" src="https://github.com/user-attachments/assets/ea08e79c-ecc2-40a7-8b35-15a2ec6ca39f" />

Query no Athena
<img width="1361" height="682" alt="query" src="https://github.com/user-attachments/assets/0457679a-6de4-4877-ae97-66c57f3b9309" />

Resultado da consulta
<img width="1347" height="674" alt="Resultado projero novo" src="https://github.com/user-attachments/assets/15827a87-fd8e-4722-86b6-18adf89e82a2" />

<img width="1340" height="679" alt="resultado final projeto 2" src="https://github.com/user-attachments/assets/c675204a-ca6e-4dd8-bbe9-f9a5faf7851f" />


👨‍💻 Autor

Projeto desenvolvido por Reginaldo Rocha
