# ☁️ Tarefas Automatizadas com AWS Lambda e Amazon S3

## 🧩 **Conceitos Principais**

### 🪄 **AWS Lambda**
O **AWS Lambda** é um serviço **serverless** que executa código **sob demanda**, sem necessidade de gerenciar servidores.  
Ele é acionado por **eventos**, como uploads em um bucket S3, mensagens em filas ou chamadas HTTP via API Gateway.  

**🔹 Características:**
- Execução de código sob demanda 🕒  
- Escalabilidade automática ⚙️  
- Cobrança apenas pelo tempo de execução 💰  
- Suporte a várias linguagens (Python, Node.js, Java, etc.) 🧠  

---

### 🗂️ **Amazon S3 (Simple Storage Service)**
O **Amazon S3** é um serviço de **armazenamento de objetos** altamente escalável e seguro, usado para guardar arquivos, backups e dados estáticos.  

**🔹 Características:**
- Armazenamento ilimitado 📦  
- Alta durabilidade (99.999999999%) 🛡️  
- Integração direta com Lambda, CloudFront e Athena 🔗  
- Permite triggers automáticos (eventos) 🎯  

---

## ⚙️ **Como a Automação Funciona**

A automação entre **S3 e Lambda** ocorre por meio de **eventos configurados no bucket S3**.  
Por exemplo:
1. Um arquivo é carregado em um bucket S3.  
2. O evento “ObjectCreated” é disparado.  
3. O **AWS Lambda** é acionado automaticamente.  
4. O código Lambda processa o arquivo (compressão, redimensionamento, análise, etc.).  
5. O resultado é salvo novamente no S3 ou enviado para outro serviço AWS.

---

## 💡 **Casos de Uso Comuns**

| 💼 Caso de Uso | 🧠 Descrição |
|----------------|--------------|
| 📸 Processamento de imagens | Redimensionar ou otimizar imagens enviadas ao S3 |
| 📊 Análise de dados | Ler arquivos CSV ou JSON enviados ao S3 e processá-los automaticamente |
| 🧾 Geração de relatórios | Automatizar a criação e o envio de relatórios periódicos |
| 🧹 Limpeza de dados | Excluir automaticamente arquivos antigos ou desnecessários |
| 🔒 Segurança | Verificar metadados e permissões de arquivos ao serem enviados |

---

## 🌍 **Importância na Arquitetura Cloud**

A automação com **Lambda + S3** representa um dos pilares da **arquitetura serverless**, trazendo benefícios como:
- **Eficiência operacional**: elimina tarefas manuais.  
- **Escalabilidade automática**: a AWS ajusta a execução conforme a demanda.  
- **Redução de custos**: paga-se apenas pelo tempo de execução do código.  
- **Maior agilidade**: ideal para pipelines de dados, integrações e microsserviços.  

---

## 🏗️ **Exemplo de Arquitetura**
Abaixo, um diagrama simplificado da arquitetura de automação com AWS Lambda e Amazon S3:


📘 **Descrição do fluxo:**
1. O usuário faz upload de um arquivo no bucket S3.  
2. O evento aciona automaticamente a função Lambda.  
3. O Lambda processa o arquivo e executa a lógica configurada.  
4. O resultado é armazenado ou encaminhado para outro serviço AWS.  




☁️ **AWS | Lambda | S3 | Serverless | Cloud Automation**
