# -Projeto-An-lise-de-Dados-com-Amazon-S3-e-Amazon-Athena

# 🚀 Projeto: Análise de Dados com Amazon S3 e Amazon Athena

## 📌 Descrição
Este projeto demonstra a criação de um fluxo simples de análise de dados na AWS utilizando Amazon S3 e Amazon Athena, permitindo consultas SQL diretamente sobre arquivos armazenados na nuvem, sem necessidade de infraestrutura.

---

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
