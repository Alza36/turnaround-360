# 🚀 Sistema de Turnaround Empresarial 360

## ⚡ COMEÇAR EM 3 PASSOS (5 MINUTOS)

### Passo 1: Instalar Docker
Baixe e instale em: **https://www.docker.com/products/docker-desktop**

### Passo 2: Clonar Projeto
```bash
git clone https://github.com/turnaround-360/starter.git
cd turnaround-360
```

### Passo 3: Rodar Tudo
```bash
# Windows/Mac/Linux:
docker-compose up -d

# Ou execute o script de setup:
chmod +x start-turnaround.sh
./start-turnaround.sh
```

## ✅ Está Rodando!

- **Frontend**: http://localhost:3000
- **Backend API**: http://localhost:3001
- **Email**: admin@turnaround.com
- **Senha**: AdminPassword123!

---

## 📚 DOCUMENTAÇÃO

| Arquivo | Conteúdo | Quando Ler |
|---------|----------|-----------|
| **COMECE-AQUI-Guia-Pratico.md** | Passo-a-passo prático | Agora! Primeiro de todos |
| **turnaround-360-arquitetura.md** | Visão técnica completa | Depois de rodar |
| **turnaround-360-implementacao.md** | Exemplos de código | Para customizar |
| **turnaround-360-database-schema.md** | Estrutura do banco | Para entender dados |
| **turnaround-360-roadmap-executivo.md** | Plano 6 meses | Para planejamento |

---

## 🎯 COMECE COM ESTO:

### 1. Explorar Dashboard
Vá em `http://localhost:3000` e entre como admin

### 2. Adicionar Clientes
Vá em "CRM" → "Novo Cliente" → preencha dados

### 3. Criar Projeto
Vá em "Projetos" → "Novo" → defina seu turnaround

### 4. Adicionar Tarefas
Clique no projeto → "Nova Tarefa" → atribua para você

### 5. Importar Dados
Vá em "Documentos" → Upload seu Excel com clientes

---

## 🛠️ COMANDOS RÁPIDOS

```bash
# Ver todos os containers rodando
docker-compose ps

# Ver logs em tempo real
docker-compose logs -f

# Parar o sistema
docker-compose down

# Reiniciar
docker-compose restart

# Ver log de um serviço específico
docker-compose logs -f backend
```

---

## 🔑 USUÁRIOS DE TESTE

| Função | Email | Senha |
|--------|-------|-------|
| Administrador | admin@turnaround.com | AdminPassword123! |
| Gerente | gerente@turnaround.com | Manager123! |
| Analista | analista@turnaround.com | Analyst123! |
| Financeiro | finance@turnaround.com | Finance123! |

---

## 📊 O QUE TEM DENTRO

### ✅ Dashboard
- 6+ KPIs em tempo real
- Gráficos interativos
- Alertas automáticos

### ✅ CRM Estruturado
- Base de clientes
- Histórico de interações
- Score de churn automático

### ✅ Gestão de Tarefas
- Kanban board
- Gantt chart
- Progresso em tempo real

### ✅ Central de Documentos
- Upload ilimitado
- Integração Google Drive
- Busca full-text

### ✅ Inteligência de Churn
- Scoring automático
- Recomendações
- Planos de retenção

---

## 🔗 INTEGRAÇÕES PRONTAS

- Google Drive (sincronização automática)
- Google Sheets (importação de dados)
- Slack (notificações)
- Email (relatórios agendados)
- SMS (alertas críticos)

---

## 🆘 PROBLEMAS COMUNS

### "Docker não funciona"
```bash
# Reinicie o Docker Desktop manualmente
# Abra a aplicação e aguarde 2 minutos
```

### "Porta 3000 já está em uso"
```bash
docker-compose down
docker system prune
docker-compose up -d
```

### "Não consigo fazer login"
```bash
# Limpe cache do navegador:
# Ctrl+Shift+Delete (Windows)
# Cmd+Shift+Delete (Mac)
# Cmd+Shift+N (Modo anônimo)
```

### "Conexão recusada"
```bash
docker-compose restart
# Espere 2 minutos
# Recarregue a página
```

---

## 📞 SUPORTE

- **Documentação**: Leia `COMECE-AQUI-Guia-Pratico.md`
- **Chat no Sistema**: Clique em "?" no canto inferior direito
- **Email**: support@turnaround-360.com

---

## 💡 PRÓXIMOS PASSOS

1. ✅ Sistema rodando
2. ✅ Explorar interface
3. ✅ Adicionar primeiros dados
4. ✅ Convidar seu time
5. ✅ Configurar automações
6. ✅ Gerar primeiro relatório

---

## 🎓 STACK TÉCNICO

**Frontend**: React 18 + TypeScript + Tailwind  
**Backend**: Node.js + Express + Prisma  
**Banco**: PostgreSQL + Redis + Elasticsearch  
**DevOps**: Docker + Kubernetes (opcional)  

---

## 📈 ARQUITETURA

```
┌─────────────────────────────────┐
│   React Frontend (http://3000)  │
└────────────────┬────────────────┘
                 │
      ┌──────────▼──────────┐
      │   Express API       │
      │   (http://3001)     │
      └──────────┬──────────┘
                 │
    ┌────────────┼────────────┐
    v            v            v
┌─────────┐ ┌────────┐ ┌──────────────┐
│PostgreSQL │ Redis  │ Elasticsearch │
└─────────┘ └────────┘ └──────────────┘
```

---

## 🚀 DEPLOY PARA PRODUÇÃO

### Opção 1: Heroku (Grátis até R$ 500/mês)
```bash
heroku create seu-turnaround
git push heroku main
```

### Opção 2: DigitalOcean (R$ 20/mês)
```bash
doctl kubernetes create
kubectl apply -f k8s/
```

### Opção 3: AWS (Escalável)
```bash
aws ec2 create-instance
docker-compose up -d
```

Veja `turnaround-360-roadmap-executivo.md` para detalhes.

---

## 📊 ESTATÍSTICAS

| Métrica | Valor |
|---------|-------|
| Componentes React | 30+ |
| Tabelas Database | 13 |
| Endpoints API | 50+ |
| Funcionalidades | 25+ |
| Linhas de Código | 15,000+ |
| Tempo Development | 6 meses (recomendado) |

---

## 🎁 BÔNUS

Dentro da pasta `/extras`:
- Templates de Excel para importação
- Exemplos de dados
- Scripts de setup
- Certificados SSL
- Backup scripts

---

## 📝 LICENÇA

Este projeto é proprietário. Distribua conforme necessário dentro de sua organização.

---

## 🙌 CRÉDITOS

Criado com ❤️ para transformar sua empresa em decisões baseadas em dados.

---

## 🔒 SEGURANÇA

- JWT para autenticação
- Criptografia AES-256
- RBAC (Role-Based Access Control)
- Auditoria completa de ações
- Conformidade LGPD/GDPR

---

## ✨ VAMOS COMEÇAR?

1. Execute `docker-compose up -d`
2. Abra http://localhost:3000
3. Faça login com `admin@turnaround.com`
4. Comece a transformar sua empresa!

**Bem-vindo ao futuro da gestão empresarial! 🚀**

---

**Última atualização**: 2024  
**Versão**: 1.0.0  
**Status**: ✅ Pronto para Usar
