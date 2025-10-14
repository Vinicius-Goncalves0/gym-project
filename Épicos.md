# Épicos

## **ÉPICO 1: Autenticação e Perfil do Usuário**

- **ID:** EPIC-01
- **Descrição:** Este épico abrange todas as funcionalidades necessárias para que um usuário possa criar uma conta, acessar o aplicativo de forma segura e ter uma identidade mínima dentro do sistema. É a porta de entrada para a experiência personalizada do GymFac.
- **Valor para o Negócio:** Garante a segurança dos dados do usuário, permite a personalização da experiência e é a base para reter informações e progresso de cada indivíduo.
- **Histórias de Usuário Potenciais:**
    - US-101: Como um novo usuário, quero me cadastrar usando e-mail e senha para poder acessar o aplicativo.
    - US-102: Como um usuário registrado, quero fazer login com minhas credenciais para acessar meus treinos.
    - US-103: Como um usuário logado, quero poder sair da minha conta (logout) para proteger minhas informações.
    - US-104: Como um usuário, quero visualizar minhas informações básicas de perfil (nome e e-mail).
    - US-105: Como um usuário que esqueceu a senha, quero solicitar a redefinição da mesma para recuperar o acesso à minha conta.

**Análise de QA:** O foco de teste aqui é multifacetado.

- **Segurança:** Validar a política de senhas fortes, o armazenamento seguro (hashing) das senhas no banco de dados e a proteção contra ataques comuns (SQL Injection, XSS) nos formulários.
- **Funcional:** Testar todo o fluxo de cadastro, login (sucesso e falha), logout e recuperação de senha.
- **Usabilidade:** Garantir que as mensagens de erro sejam claras e úteis (ex: "E-mail já cadastrado", "Senha incorreta").

## **ÉPICO 2: Gerenciamento de Treinos**

- **ID:** EPIC-02
- **Descrição:** Este é o coração funcional do aplicativo. Engloba a capacidade do usuário de criar, visualizar, modificar e remover suas rotinas de treino personalizadas.
- **Valor para o Negócio:** Entrega a principal proposta de valor do MVP – permitir que os usuários digitalizem e organizem seus planos de treino de forma simples e eficiente.
- **Histórias de Usuário Potenciais:**
    - US-201: Como um praticante de musculação, quero criar um novo treino personalizado nomeando-o e adicionando exercícios.
    - US-202: Como um usuário, quero visualizar uma lista com todos os meus treinos salvos.
    - US-203: Como um usuário, quero poder editar um treino existente para alterar seu nome ou a lista de exercícios.
    - US-204: Como um usuário, quero poder excluir um treino que não utilizo mais.

**Análise de QA:** A estratégia de teste deve focar intensamente na integridade dos dados.

- **Testes CRUD:** Validar rigorosamente as quatro operações básicas: **C**riar, **L**er (Read), **A**tualizar (Update) e **D**eletar treinos.
- **Casos de Borda:** Testar o que acontece ao tentar criar um treino sem nome, sem exercícios, com nomes muito longos ou com nomes duplicados.
- **Validação de Dados:** Garantir que os dados salvos no banco de dados correspondem exatamente ao que foi inserido na interface.

## **ÉPICO 3: Execução de Treino**

- **ID:** EPIC-03
- **Descrição:** Este épico cobre a experiência interativa do usuário "dentro da academia". Ele transforma um plano de treino estático em uma sessão de treino ativa, onde o progresso pode ser registrado em tempo real.
- **Valor para o Negócio:** Aumenta o engajamento do usuário ao fornecer uma ferramenta útil durante a atividade física, permitindo o registro preciso que alimenta o histórico de progresso.
- **Histórias de Usuário Potenciais:**
    - US-301: Como um usuário, quero iniciar uma "sessão de treino" a partir de um dos meus treinos salvos.
    - US-302: Durante uma sessão, quero visualizar a lista de exercícios e marcar cada um como concluído.
    - US-303: Para cada exercício, quero registrar o peso, o número de repetições e as séries realizadas.
    - US-304: Como um usuário, quero poder finalizar a sessão de treino, salvando-a no meu histórico.

**Análise de QA:** O foco aqui é na usabilidade e no gerenciamento de estado.

- **Testes de Usabilidade:** A interface deve ser extremamente simples e rápida de usar, considerando que o usuário estará se exercitando. Botões grandes e fluxos claros são essenciais.
- **Gerenciamento de Estado:** O que acontece se o usuário receber uma ligação, minimizar o app ou a bateria acabar no meio de um treino? O estado da sessão deve ser salvo e recuperável?
- **Performance:** A interface deve ser fluida e sem travamentos durante a execução do treino.

## **ÉPICO 4: Histórico e Acompanhamento**

- **ID:** EPIC-04
- **Descrição:** Este épico trata da capacidade do usuário de visualizar seu histórico de atividades e, consequentemente, acompanhar seu progresso ao longo do tempo.
- **Valor para o Negócio:** É um fator chave para a retenção de usuários. Ver o progresso e o histórico de trabalho duro é um dos principais motivadores para continuar usando o aplicativo.
- **Histórias de Usuário Potenciais:**
    - US-401: Como um usuário, quero acessar uma tela de histórico que lista todas as minhas sessões de treino concluídas.
    - US-402: Quero poder tocar em uma sessão de treino do meu histórico para ver os detalhes do que foi realizado (exercícios, pesos, séries, repetições).

**Análise de QA:** A precisão dos dados é a prioridade máxima.

- **Validação de Dados:** Verificar se os dados exibidos no histórico correspondem exatamente aos dados que foram inseridos durante a execução do treino.
- **Testes de Carga:** Como a tela de histórico se comporta quando o usuário tem centenas de treinos registrados? A lista carrega de forma eficiente (paginação)?
- **Apresentação:** Garantir que as informações (datas, unidades de peso, etc.) sejam exibidas de forma clara e consistente.

### **Rastreabilidade: Conectando Requisitos e Épicos**

| ID do Requisito | Descrição do Requisito | Épico Relacionado |
| --- | --- | --- |
| RF-001 | Autenticação de Usuário | EPIC-01: Autenticação e Perfil |
| RF-002 | Criação e Edição de Treinos | EPIC-02: Gerenciamento de Treinos |
| RF-003 | Visualização da Lista de Treinos | EPIC-02: Gerenciamento de Treinos |
| RF-004 | Execução de um Treino | EPIC-03: Execução de Treino |
| RF-005 | Histórico Simples de Treinos | EPIC-04: Histórico e Acompanhamento |