# Projeto Transformação DevOps — CodeFactory Solutions

![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Jardesongb/devops-codefactory/ci.yml?branch=principal&style=flat-square&label=CI%20Pipeline)
![License MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)
![Release Version](https://img.shields.io/badge/version-v0.1.0-green.svg?style=flat-square)

Documentação e implementação da proposta de modernização e padronização dos processos de software para a empresa fictícia **CodeFactory Solutions**, aplicando a **Cultura DevOps** para viabilizar versionamento estruturado, integração contínua e conteinerização.

---

## 🎯 1. Descrição do Projeto

Este repositório consolida as diretrizes e a infraestrutura básica necessárias para solucionar os problemas recorrentes de gargalos em entregas, falhas de integração pós-atualização e falta de padronização nos ambientes da **CodeFactory Solutions**. A solução adota um fluxo colaborativo baseado no *GitHub Flow*, com testes e construções automatizadas a cada *pull request* ou *commit*.

---

## 🚀 2. Objetivos Principais

* **Colaboração e Organização:** Estabelecer convenções claras de commits (*Conventional Commits*) e controle de branchs.
* **Automação (CI):** Garantir a verificação contínua do código através do GitHub Actions a cada alteração.
* **Padronização de Ambiente:** Utilizar containers Docker para eliminar o problema de divergência de ambientes entre desenvolvimento e produção.
* **Segurança Integrada:** Monitoramento de vulnerabilidades em dependências com análise contínua via Dependabot.

---

## 🛠️ 3. Tecnologias Utilizadas

| Categoria | Tecnologia | Finalidade |
| :--- | :--- | :--- |
| **Versionamento** | Git & GitHub | Controle de código-fonte, branches e revisão em equipe |
| **Containerização** | Docker | Criação e empacotamento da imagem da aplicação |
| **Automação / CI** | GitHub Actions | Esteira automatizada de verificação e build |
| **Servidor Web** | Nginx / HTML5 | Servidor leve para disponibilização da aplicação web |
| **Segurança** | Dependabot | Análise de dependências e alerta de vulnerabilidades |

---

## 📁 4. Estrutura do Repositório

```text
devops-codefactory/
├── .github/
│   └── workflows/
│       └── ci.yml          # Configuração do Pipeline de Integração Contínua (CI)
├── docker/                 # Arquivos auxiliares e configurações de infraestrutura
├── src/
│   └── index.html          # Código-fonte da aplicação web
├── .gitignore              # Arquivos ignorados pelo Git
├── Dockerfile              # Definição da imagem Docker da aplicação
├── LICENSE                 # Termos da Licença MIT do projeto
└── README.md               # Documentação principal do repositório

5. Instruções de Instalação e Execução
Pré-requisitos
Git instalado.

Docker Desktop instalado e em execução.

Passo a Passo
Clonar o Repositório:
git clone [https://github.com/Jardesongb/devops-codefactory.git](https://github.com/Jardesongb/devops-codefactory.git)
cd devops-codefactory

Execução Local via Docker (Recomendado):

# Construir a imagem Docker
docker build -t devops-codefactory .

# Executar o container na porta 8080
docker run -d -p 8080:80 --name app-codefactory devops-codefactory

6. Equipe Desenvolvedora
Jardeson Gabriel

Ana Luiza

📜 7. Licença
Este projeto está licenciado sob a Licença MIT — consulte o arquivo LICENSE para mais detalhes.

🔖 8. Histórico de Versões
v0.1.0 — Implementação inicial da estrutura de pastas, Dockerfile, pipeline de CI via GitHub Actions e documentação principal.