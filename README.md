# -Projeto-Analise-de-Dados-com-Amazon-S3-e-Amazon-Athena

## 📌 Descrição
Este projeto demonstra a criação de um fluxo simples de análise de dados na AWS utilizando Amazon S3 e Amazon Athena, permitindo consultas SQL diretamente sobre arquivos armazenados na nuvem, sem necessidade de infraestrutura.

<img width="1536" height="1024" alt="imagem projeto hoje" src="https://github.com/user-attachments/assets/6b149a3b-bd6f-4f66-a738-b10665e6e760" />


## 🧱 Arquitetura do Projeto

Fluxo:

1. Upload de arquivo CSV no Amazon S3
<img width="1359" height="675" alt="bucket scv" src="https://github.com/user-attachments/assets/06c7c692-a92f-4961-b5b6-e8f14cc3c3d3" />

2. Armazenamento dos dados na camada "dados/"
<img width="1346" height="680" alt="1" src="https://github.com/user-attachments/assets/80c133d4-8284-4ba9-b66d-8a3e95418b65" />

3. Execução de consultas SQL
<img width="1361" height="682" alt="query" src="https://github.com/user-attachments/assets/f1014fcf-76c6-4ffc-8f7f-21d0f096e1c9" />

4.  Armazenamento dos resultados no S3
<img width="1347" height="674" alt="Resultado projero novo" src="https://github.com/user-attachments/assets/2e598cf7-1b19-4675-b243-c731935c55d2" />
<img width="1340" height="679" alt="resultado final projeto 2" src="https://github.com/user-attachments/assets/b8104bb7-f061-4764-bf78-2f3a59ce7bb4" />


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
