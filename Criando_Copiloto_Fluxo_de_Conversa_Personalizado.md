# Criando um Copilot com Fluxo de Conversa Personalizado no Microsoft Copilot Studio

## 📝 Criar um Copilot em branco

1. Acesse [https://copilotstudio.microsoft.com](https://copilotstudio.microsoft.com) e faça login com sua conta Microsoft.  
2. Crie um novo projeto: na página inicial, clique em **"Criar"**.  
3. Escolha **"Novo agente"** e selecione a opção **"Ignorar para configurar"** (sem modelo pré-definido).  
4. Configure o básico:  
   - Dê um nome para seu Copilot e clique em **Criar**.  
   - Adicione uma descrição (explique a responsabilidade do chatbot).  
   - Adicione instruções (prompt que define tom, temperatura, ações etc.).  

---

## 🛠️ Customizar um tópico

Tópicos são os blocos de conversa do seu Copilot. Cada tópico define como o Copilot responde a uma intenção do usuário (perguntas, comandos ou dúvidas).

1. Com o agente criado, vá para a aba **"Tópicos"**.  
2. Tipos de tópicos:  
   - **Tópicos personalizados**: criados por você para necessidades específicas (ex: "horário de atendimento", "status de pedido").  
   - **Tópicos de sistema**: pré-configurados para funções básicas (ex: saudações, ajuda, redefinir conversa, boas-vindas, saída).  
3. Adicione um novo tópico (baseado na descrição do agente ou em branco):  
   - Inclua **frases de gatilho** (exemplos de perguntas que ativam o tópico, reconhecidas por linguagem natural).  
4. Ao finalizar o tópico, clique em **Testar** (sempre inicie uma nova conversa para testar).  
5. Se estiver tudo certo, clique em **Publicar**.  

---

## ⚠️ Como Personalizar uma Mensagem de Erro de Tópico

| Aspecto                    | Fallback                          | Conversational Boosting                             | Onde editar                             |
|----------------------------|-----------------------------------|------------------------------------------------------|------------------------------------------|
| **Quando é ativado**       | Quando o bot não entende          | Quando não há tópico correspondente, mas há fontes   | Tópico de sistema "Fallback" ou global  |
| **Tipo de resposta**       | Mensagem fixa ou redirecionamento| Resposta gerada por IA com base em fontes conectadas | Configurações > Experiência de conversa |
| **Usa IA generativa?**     | Não diretamente                   | Sim                                                  | Configurações > Experiência de conversa |
| **Personalizável?**        | Sim, texto e redirecionamento     | Sim, com fontes e instruções                         | Editor do tópico Fallback / Configurações |
| **Requer fontes externas?**| Não                                | Sim (sites, PDFs, SharePoint, Dataverse, etc.)       | Configurações > Fontes de conhecimento  |
| **Objetivo principal**     | Tratar falhas na compreensão      | Ampliar a capacidade do Copilot com IA               | Geral / Comportamento padrão             |

---

# 🎛️ Como Aumentar ou Diminuir a Qualidade da Resposta com GenAI no Copilot Studio

No Microsoft Copilot Studio, você pode ajustar o nível de **qualidade, detalhamento e objetividade** das respostas geradas por IA (GenAI) com base no comportamento do Copilot.

## ✅ Passo a passo

1. Acesse seu Copilot em [https://copilotstudio.microsoft.com](https://copilotstudio.microsoft.com) e abra seu projeto.  
2. Abra o menu **Configurações** (ícone de engrenagem no canto superior direito).  
3. Vá para **Experiência de conversa**.  
4. Localize a seção **Comportamento do Copilot** e ajuste o controle deslizante para escolher entre:  
   - **↘️ Respostas breves e diretas** — mais objetividade, menos detalhamento.  
   - **⚖️ Respostas equilibradas** — bom equilíbrio entre detalhe e agilidade.  
   - **↗️ Respostas completas e ricas** — mais contexto e explicações detalhadas.  
5. Salve as alterações.  
6. Teste no simulador enviando perguntas para verificar o comportamento.

---

## 🎯 Dicas

- Use respostas **diretas e objetivas** para atendimentos rápidos (ex: status de pedido, horários).  
- Use respostas **detalhadas e explicativas** quando o usuário esperar orientações ou suporte mais completo (ex: onboarding, suporte técnico).  


