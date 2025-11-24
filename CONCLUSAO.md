# 10. Conclusão

## Sumarização dos resultados alcançados
Ao longo do desenvolvimento do gym-project, alcançámos os objetivos principais definidos no escopo inicial. O projeto trouxe uma base funcional que inclui:
- Implementação das funcionalidades centrais para gestão (cadastro/edição) de entidades relevantes ao domínio do ginásio.
- Estrutura de código modular e organizada, facilitando manutenção e evolução.
- Documentação básica que cobre instalação, uso e contribuição.
- Testes automatizados para os componentes críticos (cobertura inicial).
- Configuração mínima de integração contínua para construir e validar o projecto em branches principais.

Esses resultados fornecem uma fundação estável para utilização prática e futuras iterações.

## Lições aprendidas durante o projeto
1. Importância do escopo bem definido: manter o escopo focado permitiu concluir funcionalidades essenciais antes de adicionar complexidade desnecessária.
2. Benefício de modularidade: separar responsabilidades (UI, lógica de domínio, persistência) tornou mais simples testar e modificar partes do sistema.
3. Testes desde cedo economizam tempo: implementar testes automatizados nas partes críticas reduziu regressões e aumentou confiança nas alterações.
4. Documentação como primeiro cidadão: documentação concisa e atualizada facilita a integração de novos contribuidores e o uso por terceiros.
5. Feedback rápido dos utilizadores: validar hipóteses com utilizadores reais logo nas primeiras versões revela prioridades reais e evita trabalho supérfluo.
6. Ferramentas de CI/CD aceleram entrega: integração contínua ajuda a detectar problemas cedo e mantém a ramificação principal em estado utilizável.

## Recomendações para projetos futuros
- Planeamento e priorização contínua:
  - Manter um backlog priorizado com histórias bem definidas e critérios de aceitação.
  - Trabalhar por iterações curtas e validar com utilizadores antes de escalar funcionalidades.
- Melhorar cobertura de testes:
  - Aumentar testes unitários e adicionar testes de integração/end-to-end para fluxos críticos.
- Automatizar deploys e ambiente:
  - Configurar pipelines para deploy automatizado (staging → produção) e scripts de infraestrutura reprodutíveis.
- Monitorização e telemetria:
  - Adicionar logging estruturado, métricas e alertas para detecção precoce de problemas em produção.
- Focar em experiência do utilizador:
  - Realizar sessões de usabilidade e melhorar acessibilidade e documentação de UI.
- Escalabilidade e performance:
  - Revisar pontos de contensão (consultas, cache, dimensionamento) conforme crescimento do uso.
- Manutenção da documentação:
  - Atualizar guias de contribuição, arquiteturas e exemplos de uso sempre que houver mudanças relevantes.
- Cultura de revisão de código:
  - Fortalecer práticas de code review e padronização (formatters, linters, convenções) para manter qualidade uniforme.
- Segurança e conformidade:
  - Fazer auditorias básicas de segurança, gerir segredos corretamente e validar requisitos legais (quando aplicável).

Conclusão breve: o projeto já oferece uma base sólida para ser utilizado e estendido. Ao seguir as recomendações acima, a equipa poderá reduzir riscos, acelerar entrega de valor e preparar a aplicação para um uso mais amplo e sustentável.