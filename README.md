# Trabalho: O Papel do Product Owner (PO) e do Scrum Master

# Arquivo de orientação: 'Arquivo de orientação para a execução do projeto.docx'


## Introdução: A Missão do Aplicativo de Treinos

Todo projeto ágil começa com uma necessidade. A nossa é clara: criar um sistema que ajude o usuário a armazenar, organizar e executar seus treinos diários. Neste trabalho, vamos detalhar o papel do **Product Owner (PO)** e do **Scrum Master** na construção deste App de Treinos.

---

## O Product Owner (PO): O Guardião do Produto

O **PO** é o "dono do produto". Ele é a voz do usuário e do negócio, e sua principal ferramenta é o **Product Backlog**, que ele constrói a partir da necessidade principal do usuário.

### Desmembrando a Necessidade em Épicos e Histórias de Usuário

O PO transforma a grande necessidade do usuário em objetivos claros e estratégicos, chamados de **épicos**.

**Épico 1: Gestão de Treinos**
* **Objetivo:** Permitir que o usuário acesse, visualize e organize seu treino diário.
* **Histórias de Usuário (US):**
    * **US:** "Como usuário, quero visualizar meu treino do dia, que foi enviado pelo meu instrutor."
        * **Critérios de Aceitação:**
            - O sistema exibe o treino agendado para o dia atual.
            - O sistema mostra o nome do treino e a data.
            - Se não houver treino, uma mensagem informativa é exibida.
    * **US:** "Como usuário, quero visualizar os exercícios do meu treino do dia, com nome, séries e repetições."
        * **Critérios de Aceitação:**
            - A lista de exercícios é exibida na ordem correta.
            - Para cada exercício, o nome, séries e repetições são visíveis.
            - Informações adicionais (ex: "descanso de 30s") também são exibidas.
    * **US:** "Como usuário, quero marcar os exercícios que já fiz para não me perder."
        * **Critérios de Aceitação:**
            - Um botão ou checkbox ao lado de cada exercício permite marcá-lo como concluído.
            - O estado de conclusão é salvo, mesmo que o usuário saia do app.

**Épico 2: Acompanhamento de Execução**
* **Objetivo:** Fornecer as ferramentas para executar e registrar os exercícios.
* **Histórias de Usuário (US):**
    * **US:** "Como usuário, quero visualizar métodos de execução dos exercícios (vídeos/textos) para fazer a forma correta."
        * **Critérios de Aceitação:**
            - O usuário pode clicar no nome do exercício para ver os detalhes.
            - A tela de detalhes exibe um vídeo de demonstração da execução.
            - Vídeos podem ser reproduzidos e pausados.

**Épico 3: Conclusão e Feedback**
* **Objetivo:** Dar ao usuário uma forma de concluir seu treino e receber feedback.
* **Histórias de Usuário (US):**
    * **US:** "Como usuário, quero marcar qual treino foi feito."
        * **Critérios de Aceitação:**
            - Um botão "Concluir Treino" aparece quando todos os exercícios são marcados.
            - O sistema salva que o treino do dia foi finalizado.
    * **US:** "Como usuário, quero receber um feedback que me informe se o treino foi concluído 100%."
        * **Critérios de Aceitação:**
            - Se todos os exercícios forem concluídos, uma mensagem de sucesso é exibida.
            - Se faltarem exercícios, o sistema informa quantos ainda precisam ser feitos.

---

## O Scrum Master: O Líder de Serviço

O **Scrum Master** é o facilitador do time. Ele não decide o que fazer, mas garante que o time consiga trabalhar de forma eficiente e sem interrupções. Ele é o **guardião do processo**.

### Ações e Resultados do Scrum Master

O resultado do trabalho do Scrum Master não é o produto final, mas sim o **desempenho e a saúde do time**.

1.  **Melhoria na Produtividade:** O Scrum Master remove obstáculos. Por exemplo, se a equipe precisa de um software específico e a compra está demorada, ele age para agilizar o processo. **O resultado é a conclusão das funcionalidades dentro do prazo.**

2.  **Autonomia da Equipe:** Ele treina a equipe para se auto-organizar. Usando as reuniões de Retrospectiva, ele guia o time para que eles mesmos identifiquem problemas (como comunicação falha) e encontrem soluções. **O resultado é um time mais proativo e independente.**

3.  **Comunicação Clara:** O Scrum Master garante que as cerimônias Scrum (como a **Daily Scrum**) sejam produtivas e curtas. **O resultado é que todos os membros do time têm uma visão clara do progresso do dia e podem se ajudar mutuamente.**

4.  **Proteção do Time:** Ele protege o time de interrupções e pedidos de última hora. Se um stakeholder pedir uma nova funcionalidade no meio da sprint, o Scrum Master intervém, garantindo que o time mantenha o foco no que foi planejado. **O resultado é a entrega consistente e sem desvios do plano inicial.**

---

## Conclusão: A Colaboração para o Sucesso

O **PO** e o **Scrum Master** trabalham em parceria para garantir o sucesso do projeto. O PO é o responsável por definir o que será feito (a estratégia, os épicos e as US) e o Scrum Master por garantir que o time tenha as melhores condições para fazer (a tática e o processo). Juntos, eles formam uma base sólida para construir e entregar um produto de alto valor.
