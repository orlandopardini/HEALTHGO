# HEALTHGO!! - A Plataforma Inteligente de Saúde

## Visão Geral

Plataforma completa de saúde e bem-estar com agentes de IA que fornecem:
- ✅ Avaliação de riscos de saúde
- 🍎 Planejamento nutricional personalizado
- 💪 Programas de treinamento personalizados
- 💰 Planejamento financeiro de saúde
- 📊 Rastreamento de progresso
- 🎨 Interface web profissional

## Instalação Rápida

### Pré-requisitos
- Python 3.10 ou superior (mas inferior a 3.14)
- Node.js 16+ e npm
- Conta Supabase (credenciais já configuradas)

### Instalação Automática (Windows)

1. **Execute o instalador:**
   ```
   install.bat
   ```

2. **Inicie a aplicação:**
   ```
   start.bat
   ```

A aplicação estará disponível em:
- **Frontend:** http://localhost:3000
- **API Backend:** http://localhost:8000

## 📁 Estrutura do Projeto

```
app/
├── frontend/              # Aplicação React
│   ├── public/           # Arquivos estáticos
│   ├── src/              # Código fonte
│   │   ├── components/   # Componentes React
│   │   ├── pages/        # Páginas da aplicação
│   │   ├── services/     # Integração com APIs
│   │   ├── styles/       # Estilos CSS
│   │   └── utils/        # Utilitários
│   └── package.json      # Dependências Node
│
├── backend/              # API e Integração CrewAI
│   ├── api/             # Endpoints FastAPI
│   ├── crews/           # Definições dos agentes
│   ├── database/        # Integração Supabase
│   └── models/          # Modelos de dados
│
├── scripts/             # Scripts de utilidade
│   ├── install.py       # Instalação automatizada
│   ├── start_backend.py # Inicia API
│   └── start_frontend.py# Inicia frontend
│
├── install.bat          # Instalador Windows
├── start.bat            # Inicializador Windows
├── requirements.txt     # Dependências Python
└── .env.example         # Exemplo de variáveis de ambiente
```

## 🔧 Configuração Manual

### 1. Backend (Python/CrewAI)

```bash
cd app/backend
pip install -r requirements.txt
```

Configure as variáveis de ambiente em `.env`:
```
OPENAI_API_KEY=sua_chave_aqui
SERPER_API_KEY=sua_chave_aqui_opcional
SUPABASE_URL=https://itrouyfcsftruntbibvv.supabase.co
SUPABASE_KEY=sua_chave_supabase
```

Inicie o backend:
```bash
python -m uvicorn api.main:app --reload --port 8000
```

### 2. Frontend (React)

```bash
cd app/frontend
npm install
npm start
```

### 3. Banco de Dados (Supabase)

Execute os scripts de migração:
```bash
cd app/backend
python database/setup_database.py
```

## 🎯 Funcionalidades

### 1. Onboarding de Usuários
- Coleta completa de dados de saúde
- Avaliação de riscos automática
- Perfil personalizado

### 2. Planos Nutricionais
- Cálculo de calorias e macronutrientes
- Sugestões de refeições
- Alternativas de alimentos
- Estimativa de custos

### 3. Programas de Treinamento
- Exercícios personalizados
- Cronogramas semanais
- Progressões gradativas
- Adaptações para equipamentos disponíveis

### 4. Planejamento Financeiro
- Análise de custos mensais
- Otimização de orçamento
- Alternativas econômicas

### 5. Rastreamento de Progresso
- Métricas de saúde
- Gráficos interativos
- Relatórios de progresso
- Insights de IA

## 🧪 Dados de Teste

A aplicação vem com perfis de usuários mockados para testes:
- Usuário 1: Profile de perda de peso
- Usuário 2: Profile de ganho muscular
- Usuário 3: Profile de manutenção de saúde
- Usuário 4: Profile com restrições médicas
- Usuário 5: Profile com orçamento limitado

## 🔒 Segurança

- ✅ Autenticação via Supabase Auth
- ✅ Dados criptografados
- ✅ Row Level Security (RLS) ativo
- ✅ Validação de entrada em todas as APIs

## 📚 Documentação da API

Após iniciar o backend, acesse:
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

---

**Desenvolvido com CrewAI, React e Supabase**

