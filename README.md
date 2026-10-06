# 🚀 EASY SWAP – E-commerce Returns Management System

EASY SWAP is a web platform designed to simplify and automate the product exchange and return process for e-commerce businesses.

---

# 🇺🇸 English

## About the Project

**EASY SWAP** is a web-based solution developed to streamline the management of product exchanges and returns in online stores.

The platform allows customers to submit exchange or return requests through a form accessed via **QR Code or link**, where they can provide order information and upload product photos.

Each request becomes a **support ticket**, which can be reviewed and managed by an operator through an **administrative dashboard**.

The system helps organize reverse logistics, reduce manual work, and improve the post-purchase experience for e-commerce customers.

---

## Objectives

- Automate exchange and return requests  
- Organize support tickets  
- Allow approval or rejection of requests  
- Generate automatic shipping codes (simulated)  
- Provide an operational dashboard with key indicators  

---

## System Type

Responsive Web Application

---

## Target Audience

- Small and medium-sized e-commerce businesses  
- Online stores using platforms such as Shopify  
- E-commerce operators managing customer support  
- Digital brands aiming to improve post-purchase experience  

---

## Technologies Used

### Frontend
- Next.js

### Backend and Database
- Supabase (PostgreSQL)

### Image Storage
- Supabase Storage

### Data Visualization
- Chart.js

### Deployment
- Vercel

---

## System Workflow

### Customer Flow

1. Customer scans a QR Code or accesses the form link
2. Fills in the request form with:
   - Order number
   - Email
   - CPF (Brazilian ID)
   - Reason for exchange
   - Description of the issue
   - Upload of up to 3 photos
   - Option to request automatic return or open a ticket only
3. Submits the request
4. The system generates a ticket in the database

---

### Support Agent Flow

1. Access the admin panel (`/admin`)
2. View the list of support tickets
3. Review information and uploaded images
4. Possible actions:
   - Approve request
   - Reject request
   - Request more information
5. If approved:
   - The system generates a simulated shipping code
   - Ticket status is updated

---

## Dashboard (Operational Indicators)

The system dashboard provides insights such as:

- Total number of tickets
- Tickets by status
- Tickets by reason
- Approval rate
- Monthly request volume

---

## Database Model (Main Tables)

### tickets
- id
- order_number
- email_cpf
- reason
- description
- status
- shipping_code
- created_at

### ticket_photos
- id
- ticket_id
- image_url

### users
- id
- email
- password
- role (admin)

---

## Deployment

The system is deployed on **Vercel**, connected to **Supabase**.

Deployment workflow:

1. Configure environment variables
2. Connect the repository to the hosting platform
3. Deploy the application
4. Generate a QR Code pointing to `/troca`

---

## Development Planning

Estimated total development time: **60 hours**

- 20 hours – Documentation
- 35 hours – Development
- 5 hours – Deployment and testing

---

## Key Features

- Automated exchange and return process for e-commerce
- Reduction of manual customer service via email or messaging
- Organized reverse logistics workflow
- Operational dashboard for decision-making

---

## Project Status

🚧 Currently in development.

---

## Author

**Elen Vieira**

Academic and portfolio project focused on building solutions for e-commerce operations.

---

# 🇧🇷 Português

## Sobre o Projeto

O **EASY SWAP** é uma solução web desenvolvida para simplificar e automatizar o processo de trocas e devoluções em lojas virtuais.

A plataforma permite que o cliente registre solicitações de troca ou devolução por meio de um formulário acessado via **QR Code ou link**, enviando informações e fotos do produto.

Essas solicitações são transformadas em **tickets**, que podem ser analisados por um atendente em um **painel administrativo**.

O sistema organiza a logística reversa, reduz retrabalho e melhora a experiência pós-venda no e-commerce.

---

## Objetivo

- Automatizar solicitações de trocas e devoluções  
- Organizar tickets de atendimento  
- Permitir aprovação ou recusa de solicitações  
- Gerar código de postagem automático (simulado)  
- Disponibilizar dashboard com indicadores operacionais  

---

## Tipo de Sistema

Aplicação Web Responsiva

---

## Público-Alvo

- Pequenos e médios e-commerces  
- Lojas virtuais que utilizam plataformas como Shopify  
- Operadores de e-commerce responsáveis pelo atendimento  
- Marcas digitais que desejam melhorar a experiência do cliente  

---

## Tecnologias Utilizadas

### Frontend
- Next.js

### Backend e Banco de Dados
- Supabase (PostgreSQL)

### Armazenamento de Imagens
- Supabase Storage

### Visualização de Dados
- Chart.js

### Deploy
- Vercel

---

## Fluxo do Sistema

### Fluxo do Cliente

1. O cliente escaneia um QR Code ou acessa o link do formulário
2. Preenche o formulário com:
   - Número do pedido
   - Email
   - CPF
   - Motivo da troca
   - Descrição do problema
   - Upload de até 3 fotos
   - Escolha entre devolução automática ou apenas abertura de ticket
3. Envia a solicitação
4. O sistema gera um ticket no banco de dados

---

### Fluxo do Atendente

1. Acessa o painel administrativo (`/admin`)
2. Visualiza a lista de tickets
3. Analisa as informações e imagens enviadas
4. Pode:
   - Aprovar
   - Recusar
   - Solicitar mais informações
5. Se aprovado:
   - O sistema gera um código de postagem (simulado)
   - O status do ticket é atualizado

---

## Dashboard (Indicadores)

O painel apresenta indicadores como:

- Total de tickets
- Tickets por status
- Tickets por motivo
- Taxa de aprovação
- Volume mensal de solicitações

---

## Modelagem do Banco (Principais Tabelas)

### tickets
- id
- numero_pedido
- email_cpf
- motivo
- descricao
- status
- codigo_postagem
- data_criacao

### fotos_ticket
- id
- ticket_id
- url_imagem

### usuarios
- id
- email
- senha
- tipo (admin)

---

## Deploy

O sistema é publicado na **Vercel**, conectado ao **Supabase**.

Fluxo de deploy:

1. Configurar variáveis de ambiente
2. Conectar o repositório à plataforma de hospedagem
3. Publicar a aplicação
4. Gerar um QR Code apontando para `/troca`

---

## Planejamento de Execução

Tempo total estimado: **60 horas**

- 20h – Documentação
- 35h – Desenvolvimento
- 5h – Deploy e testes

---

## Diferencial da Solução

- Automatização de trocas para pequenos e médios e-commerces
- Redução de atendimento manual via WhatsApp e e-mail
- Organização da logística reversa
- Dashboard estratégico para tomada de decisão

---

## Status do Projeto

🚧 Em desenvolvimento.

---

## Autora

**Elen Vieira**

Projeto acadêmico / portfólio com foco em soluções para e-commerce.
