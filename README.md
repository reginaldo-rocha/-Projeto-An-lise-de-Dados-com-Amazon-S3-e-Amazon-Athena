# -Projeto-Analise-de-Dados-com-Amazon-S3-e-Amazon-Athena

## 📌 Descrição
Este projeto demonstra a criação de um fluxo simples de análise de dados na AWS utilizando Amazon S3 e Amazon Athena, permitindo consultas SQL diretamente sobre arquivos armazenados na nuvem, sem necessidade de infraestrutura.

<img width="1536" height="1024" alt="imagem projeto hoje" src="https://github.com/user-attachments/assets/6b149a3b-bd6f-4f66-a738-b10665e6e760" />


## 🧱 Arquitetura do Projeto

Fluxo:
1. Upload de arquivo CSV no Amazon S3
<img width="1359" height="675" alt="bucket scv" src="https://github.com/user-attachments/assets/06c7c692-a92f-4961-b5b6-e8f14cc3c3d3" />

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
Ideal para análise exploratória de dado


👨‍💻 Autor

Projeto desenvolvido por Reginaldo Rocha
