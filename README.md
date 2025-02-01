# 🌡️ Transformação de Temperaturas com Web API, Docker e Azure DevOps  

Este repositório contém um projeto de **Web API** para conversão de temperaturas, desenvolvido em **Visual Studio**, utilizando **Docker** e implantado no **Azure** via **Azure DevOps Pipelines**. O objetivo é criar um fluxo de **CI/CD** eficiente e automatizado para deploy contínuo da aplicação no Azure.  

## 📌 Tecnologias Utilizadas  

- **Visual Studio** – Desenvolvimento da Web API  
- **Docker** – Containerização da aplicação  
- **Azure DevOps** – Automação do CI/CD  
- **Azure Container Registry (ACR)** – Armazenamento da imagem do Docker  
- **Azure Web App** – Hospedagem da API  
- **GitHub & Azure CLI** – Gerenciamento de código e integração com o DevOps  

## 🚀 Configuração do Projeto  

### 1️⃣ **Criando o ambiente**  

1. Criar uma conta no **Azure DevOps** e configurar uma **Organização**.  
2. No **Visual Studio**, criar uma **Web API** com suporte a **Docker**.  
3. Instalar e configurar o **Docker Desktop**.  

### 2️⃣ **Configuração do Azure**  

1. Criar um **Grupo de Recursos** no **Portal Azure**.  
2. Criar um **Azure Container Registry (ACR)** para armazenar as imagens do Docker.  
3. Criar um **Web App** para hospedar a aplicação.  

### 3️⃣ **Configuração do CI/CD com Azure DevOps**  

1. Criar um **pipeline YAML** para automação do build e deploy.  
2. Adicionar tasks para:  
   - Build da imagem Docker  
   - Registro da imagem no **ACR**  
   - Deploy no **Web App**  
3. Criar um **webhook** para atualização automática do contêiner.  
4. Atualizar as credenciais de administrador no ACR para garantir acesso ao deploy.  

### 4️⃣ **Publicação e Testes**  

1. Registrar a imagem do **Docker** no **ACR**.  
2. Apontar o repositório do **Azure DevOps** para o **GitHub** via **Azure CLI**.  
3. Fazer o deploy da aplicação.  
4. Testar a API para garantir que as atualizações ocorrem sem quedas.  

## 🛠 **Exemplo de Requisição**  

📍 **Endpoint:** `http://seu-webapp.azurewebsites.net/api/temperatura`  
📍 **Método:** **POST**  
📍 **Body (JSON):**  
```json
{
    "temperatura": 25,
    "escala": "Celsius"
}
```  
📍 **Resposta:**  
```json
{
    "kelvin": 298.15
}
```  

## 🔗 **Próximos Passos**  

- Melhorar a segurança com **autenticação e autorização**.  
- Implementar **monitoramento e logging** com **Azure Application Insights**.  
- Expandir para outras escalas de temperatura (Fahrenheit, Rankine, etc.).  

💬 **Contribuições são bem-vindas!** Caso tenha sugestões ou melhorias, abra um **Pull Request** ou entre em contato. 🚀  

---
## REFERÊNCIAS 
DIO AZ204
