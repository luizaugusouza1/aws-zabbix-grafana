# 📘 Laboratório – Deploy de Zabbix & Grafana na AWS

## 1. 🎯 Objetivo

Este laboratório tem como objetivo criar uma solução completa de **monitoramento corporativo** utilizando **Zabbix** e **Grafana**, implantados em uma infraestrutura **100% automatizada com AWS CloudFormation**.  
O projeto demonstra habilidades práticas em **Cloud, DevOps, Infraestrutura, Segurança, Automação e Versionamento**, criando um ambiente replicável, seguro e de fácil manutenção.

---

## 2. 🏗️ Arquitetura da Solução

A arquitetura foi construída utilizando recursos nativos da AWS, garantindo isolamento, resiliência e organização em camadas.

### 🔹 **Componentes Principais**

- **VPC dedicada**
  - Sub-redes públicas e privadas  
  - Tabelas de roteamento  
  - Internet Gateway  

- **Instância EC2 (Ubuntu 22.04)**
  - Zabbix Server instalado automaticamente  
  - Grafana instalado automaticamente  
  - Regras de firewall otimizadas  

- **Armazenamento EBS**
  - Volume persistente para configurações e dados  

- **Elastic IP**
  - IP estático para acesso público  

- **Security Groups**
  - Liberação de portas Zabbix, Grafana, HTTP/HTTPS e SSH  

- **User Data**
  - Script de automação para instalação dos serviços  

- **CloudFormation**
  - Deploy completo da infraestrutura como código (IaC)  

### 🔹 **Fluxo da Arquitetura**

---

## 3. 🧰 Tecnologias e Recursos Utilizados

### 🟦 **AWS**
- VPC  
- EC2  
- EBS  
- Elastic IP  
- Security Groups  
- CloudFormation  
- IAM  

### 🟧 **Infraestrutura & Automação**
- CloudFormation (YAML)  
- Bash (User Data – automação do servidor)  
- **GitHub (versionamento de código)**  
- **GitHub Desktop/CLI para commits e pushes**  
- **VS Code (edição e organização do projeto)**  
- GitHub Actions *(opcional para CI/CD)*  

### 🟩 **Monitoramento**
- Zabbix Server  
- Grafana  

### 🟨 **Linguagens & Configurações**
- YAML  
- Bash  
- JSON  

---

## 4. 🚀 Jornada de Execução e Evidências

### **4.1 – Preparação do Ambiente**
- Organização do repositório no GitHub  
- Edição do projeto utilizando **VS Code**  
- Criação dos templates CloudFormation  
- Definição das permissões de IAM para execução  

### **4.2 – Deploy da Infraestrutura**
- Upload do template no CloudFormation  
- Criação automática da VPC e sub-redes  
- Provisionamento da EC2 com EIP  
- Configuração de rotas e regras de segurança  

### **4.3 – Provisionamento Automático (User Data)**

O script automatiza:
- Atualização do sistema  
- Instalação do Zabbix Server  
- Instalação do Grafana  
- Habilitação e start dos serviços  
- Ajustes de firewall interno  

### **4.4 – Evidências (inserir prints aqui)**

Sugestões:
- Console da AWS – Stack criada  
- Recursos da VPC  
- EC2 em execução  
- Tela inicial do Zabbix  
- Tela inicial do Grafana  
- Dashboard de monitoramento  
- VS Code mostrando a estrutura do projeto  
- GitHub com commits e branches  

---

## 5. 📘 Principais Aprendizados

Durante este laboratório, foram aplicados conceitos essenciais:

- Infraestrutura como Código (IaC) com CloudFormation  
- Boas práticas de arquitetura AWS  
- Automação completa de instalação via User Data  
- Monitoramento integrado com Zabbix e Grafana  
- Segurança de rede com Security Groups  
- Armazenamento persistente com EBS  
- Versionamento e organização com **GitHub**  
- Edição e desenvolvimento do projeto utilizando **VS Code**  

---

## 6. 🔮 Próximos Passos

- Migrar banco do Zabbix para RDS MariaDB  
- Adicionar Load Balancer e Auto Scaling  
- Integrar sistemas de notificação (Slack, Teams, Email)  
- Criar pipeline CI/CD (GitHub Actions ou AWS CodePipeline)  
- Instalar Zabbix Agent em instâncias adicionais  
- Automatizar dashboards no Grafana  
- Criar módulo Terraform para comparação IaC  

---

