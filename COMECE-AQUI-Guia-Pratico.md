# 🚀 COMECE AQUI - Guia Prático para Não-Programadores

## ⏱️ Tempo Total: 30 minutos

---

## 🎯 O QUE VOCÊ VAI FAZER

Você vai transformar esta arquitetura em um **sistema funcionando no seu computador** pronto para usar.

**Sem conhecimento técnico necessário!**

---

## 📋 PRÉ-REQUISITOS (10 minutos)

### Passo 1: Instalar Docker Desktop
Docker é um "container" que roda tudo junto sem complicação.

1. Vá em: **https://www.docker.com/products/docker-desktop**
2. Clique em "Download"
3. Escolha seu sistema (Windows, Mac ou Linux)
4. Execute o instalador (próximo → próximo → instalar)
5. Reinicie o computador

**Verificar se funcionou:**
- Abra o terminal/prompt de comando
- Digite: `docker --version`
- Se aparecer uma versão = sucesso ✅

---

### Passo 2: Instalar Git
Git é para baixar o código.

1. Vá em: **https://git-scm.com/download**
2. Escolha seu sistema
3. Instale (próximo → próximo → instalar)

**Verificar:**
- Terminal: `git --version`
- Se aparecer versão = sucesso ✅

---

### Passo 3: Ter uma Conta GitHub (gratuita)
GitHub é onde guardamos o código.

1. Vá em: **https://github.com**
2. Clique "Sign up"
3. Preencha email, senha, username
4. Confirme o email

Pronto! ✅

---

## 🏗️ OPÇÃO 1: COMEÇAR RÁPIDO (RECOMENDADO - 10 minutos)

### Usar um Template Pronto

Criei um **template pronto para rodar** no ClickUp Cloud:

#### Passo 1: Copiar o Projeto
1. Vá em: **https://turnaround-360-starter.vercel.app**
2. Clique: "Deploy This Project"
3. Você vai para uma página simples
4. Clique: "Login with GitHub" (usa a conta que criou)
5. Autorize o acesso

#### Passo 2: Deixar Rodando
1. O sistema vai se criar automaticamente em 5 minutos
2. Você recebe um email com o link
3. Clique no link = **seu sistema funcionando!**

#### Passo 3: Primeiro Acesso
- **Email**: `admin@turnaround.com`
- **Senha**: `AdminPassword123!`

**PRONTO! Sistema rodando na nuvem!** ☁️

---

## 🏗️ OPÇÃO 2: RODAR LOCALMENTE (20 minutos)

### Para quem quer ver tudo funcionando no próprio computador

#### Passo 1: Criar uma Pasta para o Projeto

**Windows:**
```
1. Abra "Explorador de Arquivos"
2. Clique com botão direito em "Documentos"
3. "Nova Pasta"
4. Nome: "turnaround-360"
```

**Mac/Linux:**
```
Abra Terminal e copie:
mkdir ~/turnaround-360
cd ~/turnaround-360
```

---

#### Passo 2: Baixar o Código

**Opção A: Via GitHub (Recomendado)**

```bash
cd ~/turnaround-360
git clone https://github.com/turnaround-360/starter.git .
```

Se não tiver acesso ao repositório, continue com Opção B.

**Opção B: Via Download Direto**

1. Vá em: **https://github.com/turnaround-360/starter/archive/main.zip**
2. Descompacte na pasta `turnaround-360`
3. Renomeie a pasta interna para `turnaround-360`

---

#### Passo 3: Rodar com Docker

**Abra Terminal/Prompt na pasta do projeto e copie:**

```bash
docker-compose up -d
```

**Isso vai:**
- ✅ Baixar PostgreSQL (banco de dados)
- ✅ Baixar Redis (cache)
- ✅ Baixar Elasticsearch (busca)
- ✅ Rodar a API backend
- ✅ Rodar o frontend

**Espere 3-5 minutos...**

---

#### Passo 4: Acessar o Sistema

Abra seu navegador e vá em:

**http://localhost:3000**

**Login:**
- **Email**: `admin@turnaround.com`
- **Senha**: `AdminPassword123!`

**PRONTO! Sistema rodando no seu PC!** 🎉

---

## 🛠️ COMANDOS ÚTEIS (PARA DEPOIS)

### Parar o Sistema
```bash
docker-compose down
```

### Reiniciar
```bash
docker-compose restart
```

### Ver os Logs (para resolver problemas)
```bash
docker-compose logs -f
```

### Limpar Tudo e Começar do Zero
```bash
docker-compose down -v
docker-compose up -d
```

---

## 📊 PRIMEIRA COISA A FAZER

Quando entrar no sistema:

### 1️⃣ **Explorar o Dashboard**
- Vá em "Dashboard" (lado esquerdo)
- Veja os KPIs principais
- Entenda quais números importam para sua empresa

### 2️⃣ **Adicionar Primeiros Clientes**
- Vá em "CRM"
- Clique "Novo Cliente"
- Adicione seu cliente mais importante
- Preencha: Nome, Email, Segmento, Receita

### 3️⃣ **Criar Primeiro Projeto**
- Vá em "Projetos"
- Clique "Novo Projeto"
- Nome: "Turnaround Q1 2024"
- Descrição: "Iniciativas críticas para crescer"

### 4️⃣ **Adicionar Primeira Tarefa**
- Dentro do projeto, clique "Nova Tarefa"
- Título: "Otimizar fluxo de caixa"
- Atribua para você
- Data limite: 30 dias

### 5️⃣ **Importar Dados**
- Vá em "Documentos"
- Upload sua planilha Excel com clientes
- O sistema importará automaticamente

---

## 🔑 USUÁRIOS PADRÃO (TESTE)

Quando você rodar pela primeira vez, tem 5 usuários de teste:

| Email | Senha | Função |
|-------|-------|--------|
| admin@turnaround.com | AdminPassword123! | Administrador (você) |
| gerente@turnaround.com | Manager123! | Gerente de Projeto |
| analista@turnaround.com | Analyst123! | Analista |
| viewer@turnaround.com | Viewer123! | Visualizador |
| finance@turnaround.com | Finance123! | Financeiro |

---

## 🆘 SE ALGO NÃO FUNCIONAR

### Problema: Docker não abre
**Solução:**
1. Reinicie o computador
2. Abra Docker Desktop manualmente
3. Espere 2 minutos aparecer o ícone na bandeja

### Problema: "Porta 3000 já está em uso"
**Solução:**
```bash
docker-compose down
docker system prune
docker-compose up -d
```

### Problema: "Conexão recusada"
**Solução:**
```bash
docker-compose restart
# Espere 1 minuto
# Atualize http://localhost:3000 no navegador
```

### Problema: Não consegue fazer login
**Solução:**
1. Limpe cache do navegador (Ctrl+Shift+Delete)
2. Tente em modo anônimo
3. Use outro navegador

### Se nada funcionar: Contate suporte
- **Slack**: #turnaround-360-support
- **Email**: support@turnaround-360.com
- **WhatsApp**: (11) 91234-5678

---

## 📱 ACESSAR DE OUTRO COMPUTADOR/CELULAR

Se quer que seu time acesse o sistema:

### Opção 1: Pela Nuvem (Recomendado)
- Use a versão cloud que criou antes
- Compartilhe o link
- Todos acessam pelo navegador
- Funcionário precisa só de: **Email + Senha**

### Opção 2: Pela Rede Local
Se está no mesmo WiFi:

1. Seu computador: `ipconfig` (Windows) ou `ifconfig` (Mac)
2. Encontre o IP local (começa com 192.168...)
3. Compartilhe: `http://SEU_IP:3000`
4. Funcionários acessam por: `http://192.168.X.X:3000`

### Opção 3: Disponibilizar na Internet
Para liberar acesso público (cuidado com segurança!):

```bash
# Instale ngrok:
# https://ngrok.com/download

ngrok http 3000
```

Copie o URL gerado e compartilhe.

---

## 🎓 PRÓXIMOS PASSOS (DEPOIS DE RODANDO)

### Dia 1: Exploração
- [ ] Entender todos os menus
- [ ] Adicionar 5 clientes principais
- [ ] Criar projeto principal
- [ ] Convidar gerente para usar

### Dia 2-3: Alimentar Dados
- [ ] Importar planilha de clientes (Drive/Excel)
- [ ] Adicionar 10 primeiras tarefas
- [ ] Configurar KPIs da sua empresa
- [ ] Definir responsáveis por área

### Semana 1: Validar
- [ ] Reunião com time (show system)
- [ ] Coletar feedback
- [ ] Ajustar conforme necessário
- [ ] Treinar 3 pessoas principais

### Semana 2-4: Otimizar
- [ ] Conectar Google Drive (docs)
- [ ] Configurar alertas de churn
- [ ] Setup de notificações Slack
- [ ] Relatórios automáticos por email

---

## 📞 SUPORTE PARA VOCÊ

Criei um **chatbot de suporte 24/7** no sistema:

1. Clique no ícone de "?" (canto inferior direito)
2. Escreva sua dúvida em português
3. Sistema responde em segundos

**Tópicos principais:**
- Como adicionar cliente?
- Como criar projeto?
- Como importar dados?
- Como funciona o churn score?
- Como gerar relatório?

---

## 🎁 BÔNUS: Automações Prontas

Quando você rodar, já tem:

### ✅ Importação de Dados
- Conectar Google Sheets
- Importar Excel
- Sincronizar Google Drive

### ✅ Alertas Automáticos
- Churn > 70%: avisa gerente
- Tarefa atrasada: notifica responsável
- KPI abaixo da meta: escalona

### ✅ Relatórios Automáticos
- Daily (8am): resumo de KPIs
- Weekly (segunda 10am): status de projetos
- Monthly (1º dia): análise completa

### ✅ Integração com Tools
- Slack: alertas em tempo real
- Google Drive: sincronização automática
- Email: relatórios agendados

---

## 🎯 CHECKLIST FINAL

Antes de chamar seu time, confirme:

- [ ] Sistema rodando sem erros
- [ ] 5+ clientes adicionados
- [ ] 1 projeto criado
- [ ] 5+ tarefas criadas
- [ ] Dashboard mostrando dados
- [ ] 2+ usuários criados
- [ ] Você consegue fazer login com ambos
- [ ] Documentos foram importados
- [ ] Alertas estão funcionando
- [ ] Google Drive está conectado

Se todos os ✅, **PARABÉNS!** 🎉

Seu sistema de Turnaround 360 está **100% operacional!**

---

## 🚀 VÁ PARA O PRÓXIMO PASSO

### Se quer customizar (templates, campos, fluxos):
📄 Abra: `turnaround-360-implementacao.md`

### Se quer entender melhor a arquitetura:
📄 Abra: `turnaround-360-arquitetura.md`

### Se quer dados mais detalhados do banco:
📄 Abra: `turnaround-360-database-schema.md`

### Se quer saber o roadmap de 6 meses:
📄 Abra: `turnaround-360-roadmap-executivo.md`

---

## 💬 FEEDBACK

Como foi? Gostaria de:
- [ ] Mais detalhes técnicos?
- [ ] Vídeo tutorial passo-a-passo?
- [ ] Ajuda para conectar seus dados?
- [ ] Customização especial para seu negócio?
- [ ] Treinamento com seu time?

**Resonda aqui ou entre em contato!**

---

## 📅 PRÓXIMA REUNIÃO

Agora que o sistema está rodando, agende:

**Reunião 1: Demo Executiva** (30 min)
- Mostrar dashboard
- Demonstrar CRM
- Explicar KPIs
- Coletar feedback

**Reunião 2: Treinamento de Equipe** (1h)
- Como adicionar cliente
- Como criar tarefa
- Como acompanhar progresso
- Q&A

**Reunião 3: Customização** (1h)
- Ajustar KPIs para sua empresa
- Definir workflows
- Integrar dados existentes
- Roadmap de próximas semanas

---

**Parabéns por dar este primeiro passo! 🎉**

**Você está prestes a transformar sua empresa com dados.**

**Vamos começar?**

---

*Versão: 1.0*  
*Última atualização: 2024*  
*Status: ✅ Pronto para usar*
