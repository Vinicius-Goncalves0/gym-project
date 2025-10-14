# GymFac

**Documento de Visão e Escopo do Projeto: GymFac**

**Versão:** 1.0

**Data:** 12 de outubro de 2025

# **1. Introdução**

### **Objetivo do Documento**

Este documento tem como objetivo formalizar a visão, o escopo, os requisitos e o planejamento inicial para o desenvolvimento do aplicativo móvel "GymFac". Ele servirá como um guia estratégico para a equipe de desenvolvimento, stakeholders e para o processo de garantia de qualidade, assegurando que todos os envolvidos compartilhem de um entendimento comum sobre os objetivos e limites do projeto.

### **Contextualização do Projeto de Engenharia de Software**

O projeto GymFac será desenvolvido utilizando uma metodologia ágil, Scrum, com sprints de duas semanas. O foco será na entrega de um Produto Mínimo Viável (MVP) que entregue valor real aos usuários finais, permitindo a coleta de feedback para guiar as iterações futuras. A equipe será multifuncional, composta por um Product Owner, um Scrum Master, Desenvolvedores e um Analista de QA.

### **Descrição do Problema a ser Resolvido**

Praticantes de musculação, especialmente os de nível iniciante a intermediário, frequentemente enfrentam dificuldades em organizar e acompanhar suas rotinas de treino. As soluções comuns (planilhas de papel, blocos de notas ou aplicativos excessivamente complexos e repletos de anúncios) são ineficientes e desmotivadoras. Falta no mercado uma ferramenta digital limpa, intuitiva e focada exclusivamente na criação, execução e acompanhamento de treinos.

### **Justificativa para o Desenvolvimento do Software**

O desenvolvimento do GymFac justifica-se pela crescente demanda por soluções de fitness digital e por uma clara oportunidade de mercado para um aplicativo que prioriza a simplicidade e a experiência do usuário. Ao oferecer uma solução gratuita e de alta usabilidade para o problema central de gerenciamento de treinos, o GymFac pode construir uma base de usuários leal, abrindo portas para futuras funcionalidades premium e modelos de monetização.

# **2. Planejamento do Projeto**

### **2.1 Escopo do Projeto**

O escopo do MVP do GymFac está focado em entregar o ciclo completo de gerenciamento de um treino.

- Funcionalidades Principais:
    - **RF-001:** Autenticação de Usuário (Cadastro, Login, Logout).
    - **RF-002:** Criação e Edição de Treinos Personalizados (Adicionar/Remover exercícios de uma lista pré-definida).
    - **RF-003:** Visualização da Lista de Treinos salvos.
    - **RF-004:** Execução de um Treino (Marcar séries, pesos e repetições realizadas).
    - **RF-005:** Histórico Simples de Treinos executados.
- Limites e Restrições:
    - Funcionalidades sociais (compartilhamento de treinos, seguir amigos).
    - Planos de dieta ou contagem de calorias.
    - Integração com wearables (smartwatches, etc.).
    - Vídeos ou GIFs demonstrando exercícios.
    - Criação de exercícios customizados pelo usuário.

### **Estabelecer os Recursos Necessários:**

- **Equipe de Desenvolvimento:**
    - 1 Product Owner (PO)
    - 1 Scrum Master / Project Manager (PM)
    - 2 Desenvolvedores Mobile (React Native)
    - 1 Desenvolvedor Backend (Node.js)
    - 1 Analista de QA
- **Tecnologias:**
    - **Mobile:** React Native.
    - **Backend:** Node.js com framework Express.js.
    - **Banco de Dados:** PostgreSQL.
    - **Autenticação:** JWT (JSON Web Tokens).
- **Infraestrutura:**
    - Serviços em nuvem (AWS ou Google Cloud).
    - Ambientes separados: Desenvolvimento, Testes/Staging e Produção.
    - Repositório de código: Git (GitHub).
    - Pipeline de CI/CD: GitHub Actions.

### **Elaborar o Cronograma do Projeto (Alto Nível):**

- **Semana 1-2 (Sprint 0):** Planejamento, setup de ambiente, design de arquitetura, prototipação (UI/UX).
- **Semana 3-10 (4 Sprints de 2 semanas):** Desenvolvimento iterativo das funcionalidades do MVP.
- **Semana 11:** Testes de ponta-a-ponta, testes de regressão e preparação para o lançamento.
- **Semana 12:** Lançamento do MVP nas lojas de aplicativos.

## **2.2 Análise de Requisitos**

### **Levantamento de Requisitos:**

- Coleta realizada através de entrevistas com 5 praticantes de academia e 2 personal trainers.
- Análise de concorrentes (apps mais populares e suas avaliações nas lojas).
- Sessões de brainstorming com a equipe do projeto.

### **Documentação dos Requisitos:**

- **Requisitos Funcionais (RF):** Os RFs estão listados na seção de escopo. Cada um será detalhado em User Stories específicas no backlog do produto.
- **Requisitos Não Funcionais (RNF):**
    - **RNF-001 (Performance):** O tempo de carregamento de qualquer tela não deve exceder 2 segundos em uma conexão 4G.
    - **RNF-002 (Usabilidade):** O fluxo de criação de um novo treino deve ser concluído em menos de 5 passos.
    - **RNF-003 (Segurança):** Senhas devem ser armazenadas utilizando hashing (ex: bcrypt). A comunicação com o servidor deve ser via HTTPS.
    - **RNF-004 (Compatibilidade):** O aplicativo deve ser compatível com as 2 últimas versões majoritárias do iOS e Android.

### **Analisar, Verificar e Priorizar os Requisitos:**

- A validação será feita através da apresentação de protótipos navegáveis (Figma) para os stakeholders.
- A priorização seguirá o método MoSCoW, onde todas as funcionalidades listadas no escopo do MVP são classificadas como **Must-Have** (Obrigatórias).

## **2.3 Estimativas**

- **Estimativa de Custo (Exemplo):** Considerando a equipe e o cronograma de 3 meses, uma estimativa inicial para o custo de desenvolvimento do MVP seria entre **R$ 180.000 e R$ 250.000**, incluindo salários, custos de infraestrutura e licenças de software.
- **Estimativa de Prazo:** O prazo estimado para a entrega do MVP é de **12 semanas (3 meses)**, conforme o cronograma de alto nível.
- **Avaliação de Recursos Necessários:** A equipe definida na seção 2.1 é considerada adequada para cumprir o escopo no prazo estimado. Não há necessidade de hardware especializado.

## **2.4 Riscos**

- Identificação dos Principais Riscos:
    1. **Técnico:** Performance abaixo do esperado em dispositivos Android mais antigos e fragmentados. (Probabilidade: Média, Impacto: Alto)
    2. **Escopo:** Solicitações de novas funcionalidades ("scope creep") durante o desenvolvimento do MVP. (Probabilidade: Alta, Impacto: Alto)
    3. **Cronograma:** Atraso na definição do UI/UX, impactando o início do desenvolvimento. (Probabilidade: Média, Impacto: Médio)
    4. **Recursos:** Saída de um membro chave da equipe de desenvolvimento. (Probabilidade: Baixa, Impacto: Alto)
- Estratégias de Mitigação:
    1. **Mitigação (Risco Técnico):** Realizar testes de performance contínuos em emuladores de dispositivos de baixo desempenho e em pelo menos um aparelho físico popular de entrada.
    2. **Mitigação (Risco de Escopo):** Manter um backlog priorizado e um processo formal de controle de mudanças gerenciado pelo PO. Ser rigoroso com a definição de "feito".
    3. **Mitigação (Risco de Cronograma):** Envolver a equipe de desenvolvimento nas fases iniciais de design para garantir a viabilidade técnica das propostas.
    4. **Mitigação (Risco de Recursos):** Manter a documentação do projeto atualizada e promover o compartilhamento de conhecimento dentro da equipe.

## **2.5 Plano de Projeto (GitHub Projects)**

O plano tático do projeto será gerenciado usando o GitHub Projects para fornecer visibilidade e rastreabilidade.

- **Cronograma de Atividades:** O projeto será dividido em **Épicos** (ex: "Autenticação", "Gerenciamento de Treinos"). Cada Épico será quebrado em **User Stories** (ex: "Criação de Treino Personalizado"). As User Stories serão decompostas em **Tarefas** (ex: "Criar endpoint da API para salvar treino", "Desenvolver tela de criação de treino", "Testar fluxo de criação de treino").
- **Atribuição de Responsabilidades:** Cada tarefa será atribuída a um membro específico da equipe dentro da ferramenta. O Analista de QA será responsável por criar e vincular as tarefas de teste a cada User Story.
- **Definição de Marcos e Entregáveis:**
    - **Marco 1 (Fim da Sprint 0):** Arquitetura definida e ambientes configurados. Protótipo de alta fidelidade aprovado.
    - **Marco 2 (Fim da Sprint 2):** Funcionalidade de autenticação e criação de treinos concluída e testada.
    - **Marco 3 (Fim da Sprint 4):** MVP completo em ambiente de Staging, pronto para a fase final de testes.
    - **Marco 4 (Fim da Semana 12):** MVP publicado nas lojas de aplicativos.