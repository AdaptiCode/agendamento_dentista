# 🦷 Agendamento — Clínica Sorriso Vida

Protótipo visual de um sistema de **agendamento online para clínica odontológica**, desenvolvido inicialmente em **HTML, CSS e JavaScript** com o objetivo de demonstrar ao cliente como será o fluxo e a experiência de utilização do produto.

> ⚠️ **Este projeto é uma demonstração/protótipo. Não representa a arquitetura final do sistema de produção.**

---

## 🎯 Objetivo deste projeto

Este protótipo foi desenvolvido para apresentar visualmente ao cliente:

* Como será a página da clínica;
* Como o paciente poderá conhecer os serviços;
* Como será realizado o agendamento;
* Como o usuário escolherá data e horário;
* Como será apresentada a confirmação;
* Como será a experiência do paciente no celular;
* Como poderá funcionar o fluxo de atendimento online.

A finalidade principal é **validar a ideia, o design e o fluxo do sistema antes do desenvolvimento completo**.

---

## 🧪 Tecnologia utilizada neste protótipo

Este repositório foi desenvolvido de forma propositalmente simples utilizando:

* HTML
* CSS
* JavaScript

A utilização dessas tecnologias neste protótipo tem como objetivo permitir uma apresentação rápida do produto ao cliente.

### Importante

O sistema apresentado aqui **não deve ser considerado a versão definitiva do produto**.

Na versão final, o projeto será desenvolvido utilizando uma arquitetura moderna, escalável e preparada para produção.

---

# 🚀 Arquitetura prevista para a versão final

A versão definitiva do sistema deverá utilizar:

## Frontend

* Next.js 16
* React
* TypeScript
* Tailwind CSS
* Componentização reutilizável
* Interface responsiva
* Mobile First

O Next.js será responsável pela aplicação web, páginas públicas, painel administrativo e experiência do paciente.

---

## 🗄️ Banco de dados

Será utilizado:

* PostgreSQL
* Prisma ORM
* TypeScript

O banco de dados deverá armazenar informações como:

* Clínica
* Profissionais
* Especialidades
* Serviços
* Pacientes
* Agendamentos
* Horários disponíveis
* Horários bloqueados
* Status dos agendamentos
* Histórico de atendimentos
* Configurações da clínica
* Usuários administrativos

---

# 📱 Integração com WhatsApp

Uma das funcionalidades previstas para a versão de produção será a integração com WhatsApp.

O sistema poderá utilizar o WhatsApp para:

* Confirmar agendamentos;
* Enviar lembretes;
* Avisar sobre alterações de horário;
* Informar cancelamentos;
* Enviar mensagens automáticas para pacientes;
* Reduzir faltas nos agendamentos.

Exemplo de fluxo:

```text
Paciente realiza agendamento
        ↓
Sistema salva o agendamento
        ↓
Agendamento é confirmado
        ↓
WhatsApp envia confirmação
        ↓
Próximo do horário
        ↓
WhatsApp envia lembrete
```

---

# ⚙️ Backend

Dependendo da complexidade e dos requisitos da versão final, poderá ser utilizado um backend separado com:

* Node.js
* Fastify
* TypeScript
* Zod
* Prisma
* PostgreSQL

O backend separado será especialmente interessante caso o sistema precise trabalhar com:

* Webhooks;
* Integração com WhatsApp;
* Filas de mensagens;
* Processamentos assíncronos;
* Integrações externas;
* Jobs automáticos;
* Múltiplas aplicações consumindo a mesma API;
* Controle centralizado de regras de negócio.

Para uma aplicação menor, parte dessas funcionalidades também poderá ser implementada diretamente no ecossistema do Next.js.

---

# 🔄 Fluxo previsto do sistema

```text
Paciente
   ↓
Página da Clínica
   ↓
Escolhe Serviço
   ↓
Escolhe Profissional
   ↓
Escolhe Data
   ↓
Escolhe Horário
   ↓
Informa seus dados
   ↓
Confirma Agendamento
   ↓
Banco de Dados
   ↓
Confirmação
   ↓
WhatsApp
   ↓
Lembrete automático
```

---

# 🏗️ Evolução do projeto

Este protótipo representa a **primeira etapa do projeto**.

### Etapa 1 — Protótipo

* HTML
* CSS
* JavaScript
* Demonstração visual
* Validação do fluxo com o cliente

### Etapa 2 — Aplicação real

* Next.js 16
* React
* TypeScript
* Banco de dados
* Prisma
* Autenticação
* Painel administrativo
* Gerenciamento de profissionais
* Gerenciamento de serviços
* Gerenciamento de horários
* Agendamentos reais

### Etapa 3 — Integrações

* WhatsApp
* Notificações
* Webhooks
* Confirmações automáticas
* Lembretes
* Integrações externas

### Etapa 4 — Produção

* Segurança
* Logs
* Monitoramento
* Backup
* Controle de permissões
* Otimização
* Deploy
* Escalabilidade

---

# 📌 Observação importante

O objetivo deste repositório é **demonstrar o conceito do produto ao cliente**.

A interface, os fluxos e as ideias apresentadas neste protótipo poderão ser utilizados como referência para o desenvolvimento da aplicação definitiva.

A versão de produção será desenvolvida separadamente, com arquitetura baseada em **Next.js 16, TypeScript, Prisma, banco de dados e integrações necessárias**, podendo utilizar um backend independente em **Node.js + Fastify + Zod** quando a complexidade do projeto justificar.

---

## 🦷 Projeto

**Clínica Sorriso Vida**

Este protótipo serve como referência visual e funcional para a futura plataforma de agendamento online da clínica.

---

## 🎛️ Prévia personalizada para o cliente

Esta demo tem um editor embutido para montar, em minutos, uma prévia com a cara do negócio do cliente.

1. Abra a demo publicada com **`?editar`** no final do endereço (ex.: `https://seu-dominio/?editar`). O editor só aparece para você; o visitante comum não vê nada. Para desligar: `?editar=0`.
2. Troque **logo, nome, subtítulo, cor, WhatsApp, Instagram, endereço, horários de atendimento, serviços e equipe**. Os horários mudam de verdade os dias e os horários disponíveis no agendamento.
3. Em **Prévia para o cliente**, informe o nome do cliente e a validade. A prévia mostra uma faixa "PRÉVIA · não é a entrega final" (contrato, cláusula 5.3) e esconde os avisos de demonstração.
4. Envie ao cliente:
   - **Copiar link**: gera um endereço com tudo que você configurou (sem precisar publicar nada novo).
   - **Baixar HTML**: arquivo único com a prévia, pronto para hospedar ou enviar.

O que você edita fica salvo só no seu navegador; use **Restaurar** para voltar ao padrão da demo.

### Ordem do agendamento

- **Barbearia e salão:** profissional primeiro, depois o serviço (só os que aquele profissional faz) e o horário.
- **Dentista e estética:** serviço primeiro, depois o profissional (só quem faz aquele serviço) e o horário.
- Nos dois casos há **"Sem preferência"** (fica com o primeiro profissional livre) e o **horário vem por último**, calculado pela duração do serviço e pela agenda de quem atende.
- Dá para inverter a ordem no editor, em *Serviços e equipe → Ordem do agendamento*.

### Formato dos campos de texto (um por linha)

- Serviços: `Nome | duração | preço` (ex.: `Corte | 30 min | R$ 45`)
- Equipe: `Nome | especialidade | serviços que faz | foto (link) | WhatsApp`. Em "serviços que faz", separe por vírgula usando os mesmos nomes da lista de serviços; vazio = faz todos. Foto e WhatsApp são opcionais; sem foto aparece a inicial do nome.
- Sem nenhuma pessoa na equipe, a etapa de profissional some.

### Confirmação pelo WhatsApp do profissional

Se o profissional tiver WhatsApp cadastrado (ou, na falta dele, o WhatsApp do negócio no editor), o botão **Confirmar e enviar no WhatsApp** abre a conversa com ele já com a mensagem pronta (cliente, telefone, serviço, profissional, data, horário, observações e um código `AG-…`). Com "Sem preferência", vale o número de quem foi atribuído ao horário. O agendamento só chega ao profissional quando o cliente toca em enviar no WhatsApp. Sem nenhum número configurado (demo pura), nada é aberto e a tela final só mostra a mensagem de exemplo.

