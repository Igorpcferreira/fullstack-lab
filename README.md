# Fullstack Lab - LAB02 com Docker Compose

📌 **Observação importante:**  
As evidências práticas da execução do laboratório **não estão neste README diretamente**.  
Elas foram organizadas em um documento PDF que pode ser encontrado na pasta [`/docs`](./docs):

➡️ [Evidências do LAB02 - Fullstack](./docs/Evidencias_LAB02_Fullstack.pdf)

---

## 🚀 Sobre o Projeto

Este repositório contém a entrega do **LAB02 - Ambiente de Desenvolvimento com Docker Compose**, que consiste em um ambiente full-stack completo:

- **Frontend:** React + Vite  
- **Backend:** NestJS  
- **Banco de Dados:** PostgreSQL (com volume persistente)  
- **Admin do Banco:** pgAdmin  
- **Proxy Reverso:** Nginx para roteamento entre frontend e backend  

---

## 📂 Estrutura

```
fullstack-lab/
├── backend/        # Código do backend (NestJS)
├── frontend/       # Código do frontend (React + Vite)
├── nginx/          # Configuração do Nginx
├── docs/           # Evidências em PDF
├── docker-compose.yml
├── .env.example
└── README.md
```

---

## 🛠️ Como rodar o projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/SEU_USUARIO/fullstack-lab.git
   cd fullstack-lab
   ```

2. Configure o arquivo `.env` a partir do `.env.example`.

3. Suba os serviços com:
   ```bash
   docker compose up --build
   ```

4. Acesse:
   - Frontend: [http://localhost:8080](http://localhost:8080)  
   - Backend: [http://localhost:8080/api](http://localhost:8080/api)  
   - pgAdmin: [http://localhost:5050](http://localhost:5050)  
   - PostgreSQL: `localhost:5432`

---

## ✅ Critérios atendidos

- Ambiente sobe com único comando (`docker compose up`).  
- Hot reload funcionando para frontend e backend.  
- Roteamento via Nginx (`/ → frontend`, `/api → backend`).  
- Banco de dados persistente.  
- Evidências organizadas em PDF na pasta `/docs`.  

---

👨‍💻 Autor: *Igor Ferreira*
