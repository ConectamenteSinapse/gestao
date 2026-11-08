# ConectaMente — Proposta de Planejamento da Sprint Final

**Projeto:** ConectaMente — Jogo Sério para Auxiliar Pessoas com Síndrome de Down nas Tarefas Diárias  
**Instituição:** FATEC Registro  
**Disciplina:** Gestão de Agilidade e Projetos de Software (GAPS)  
**Atividade:** AT2 — SWOT e Planejamento da Sprint Final  
**Milestone:** `Sprint Final - Entrega da Banca`  
**Prazo:** 15/11/2026  
**Situação:** Proposta individual para avaliação da equipe e da Product Owner

## 1. Objetivo da Sprint Final

Consolidar e verificar as funcionalidades essenciais do ConectaMente para apresentar à banca uma demonstração do fluxo principal do sistema.

A Sprint Final prioriza a estabilidade da aplicação, a documentação das decisões estratégicas e a preparação da apresentação, evitando ampliar o escopo com funcionalidades que não possam ser concluídas e testadas dentro do prazo.

O planejamento utiliza a Análise SWOT e a Matriz TOWS documentadas no repositório `gestao` como base para as decisões.

## 2. Fluxo principal demonstrável

O fluxo previsto para apresentação considera as duas jornadas descritas no artigo do projeto.

### Jornada do responsável

1. Acessar o sistema e realizar login.
2. Cadastrar ou vincular o perfil de uma criança.
3. Acessar as informações e configurações disponíveis.
4. Consultar o histórico ou progresso registrado após a atividade.

### Jornada da criança

1. Acessar seu perfil.
2. Selecionar o personagem, caso a funcionalidade esteja disponível.
3. Escolher um cômodo ou desafio.
4. Realizar uma atividade do jogo.
5. Receber o feedback da resposta.
6. Concluir a atividade e registrar o progresso.

**Critério para a apresentação:** o fluxo deverá ser demonstrado conforme as funcionalidades efetivamente implementadas e verificadas. Etapas ainda não disponíveis não serão apresentadas como concluídas.

## 3. Priorização MoSCoW

As prioridades abaixo representam uma proposta de escopo para a Sprint Final.

| Classificação | Funcionalidades e atividades | Justificativa |
|---|---|---|
| **Must Have** | Acesso ao sistema, vinculação da criança, execução de pelo menos uma atividade funcional, feedback e registro de progresso necessários ao fluxo demonstrável | Constituem o caminho principal da aplicação e são essenciais para apresentar o funcionamento do projeto. |
| **Must Have** | Verificação técnica do fluxo principal e correção de falhas que impeçam a demonstração | Reduz o risco de falhas durante a apresentação. |
| **Must Have** | Revisão da SWOT, TOWS e documentação exigida pela AT2 | Necessária para comprovar o planejamento estratégico solicitado pela disciplina. |
| **Should Have** | Melhorias de clareza nas orientações existentes e preparação de recomendações visuais e sonoras | Contribuem para a usabilidade, mas o tutorial completo será planejado para outra etapa. |
| **Could Have** | Ajustes visuais complementares e melhorias não impeditivas | Podem ser realizados se houver capacidade após a conclusão dos itens essenciais. |
| **Won't Have nesta Sprint** | Versão mobile completa, tutorial completo com áudio e imagens, integração com CMS e validação com crianças do público-alvo | Dependem de desenvolvimento adicional, disponibilidade de participantes ou tempo de avaliação incompatível com o planejamento proposto. |

A classificação Won't Have não representa o cancelamento definitivo das funcionalidades, mas seu adiamento para uma etapa futura.

## 4. Cortes de escopo e justificativas

### 4.1. Versão mobile completa

**Decisão proposta:** manter a demonstração na versão desktop e adiar a adaptação mobile completa.

**Justificativa:** a limitação atual da plataforma, identificada na SWOT como W1, combinada com o prazo fixo da banca (T1), recomenda concentrar os esforços na versão demonstrável.

**Relação TOWS:** estratégia WT — Sobrevivência.

### 4.2. Tutorial inicial com imagens e áudio

**Decisão proposta:** registrar os requisitos do tutorial e adiar sua implementação completa.

**Justificativa:** a ausência de orientações iniciais (W2) é uma fraqueza identificada. Os profissionais envolvidos na pesquisa de personas podem contribuir para definir orientações mais adequadas antes da implementação.

**Relação TOWS:** estratégia WO — Reforço.

### 4.3. Validação com o público-alvo

**Decisão proposta:** planejar os testes de usabilidade com crianças com síndrome de Down para uma etapa posterior.

**Justificativa:** a equipe ainda não realizou essa validação (W3), e a disponibilidade de participantes dentro do prazo representa um risco externo (T5).

Testes funcionais com outros participantes poderão verificar o funcionamento técnico, mas não substituirão a validação com o público-alvo.

## 5. Gestão de riscos e contingências

| Risco | Impacto | Ação preventiva | Contingência |
|---|---|---|---|
| API do Render em repouso ou indisponível | O sistema não consegue acessar funcionalidades dependentes do backend | Acessar a API com antecedência e verificar os endpoints necessários | Utilizar demonstração gravada do fluxo principal, caso permitido pela banca |
| Falha de internet na apresentação | Impossibilidade de acessar serviços hospedados na nuvem | Verificar a conexão e preparar previamente os recursos da apresentação | Apresentar vídeo demonstrativo e documentação técnica |
| Falha funcional durante a demonstração | Interrupção da jornada apresentada | Executar testes do fluxo principal antes da banca | Demonstrar as etapas disponíveis e explicar a limitação identificada, sem afirmar que o fluxo completo funcionou |
| Prazo insuficiente para concluir melhorias | Funcionalidades incompletas na entrega | Concentrar esforços nos Must Have e evitar novas funcionalidades | Adiar itens Should Have e Could Have, registrando os cortes de escopo |
| Indisponibilidade de participantes do público-alvo | Ausência de validação de usabilidade com crianças | Buscar contato antecipado com instituições e profissionais | Realizar testes técnicos com outros participantes e planejar a validação adequada para o próximo semestre |

## 6. Organização no GitHub Projects

O acompanhamento da Sprint Final será realizado no GitHub Projects do ConectaMente, utilizando:

- **Milestone:** `Sprint Final - Entrega da Banca`.
- **Status:** Backlog, Ready, In progress, In review e Done.
- **Priority:** classificação de importância ou urgência da tarefa.
- **MoSCoW:** definição de escopo para a entrega.
- **Estimate:** estimativa de esforço utilizada pela equipe.
- **Assignees:** responsáveis pelas atividades.
- **Critérios de aceitação e DoD:** condições para considerar cada Issue concluída.

As atividades devem ser vinculadas à Milestone e acompanhadas até sua conclusão ou adiamento formal.

## 7. Critérios para considerar a Sprint Final preparada

- [ ] Fluxo principal selecionado e verificado tecnicamente.
- [ ] Falhas impeditivas identificadas e tratadas ou explicitamente registradas.
- [ ] SWOT contendo pelo menos três fatores por quadrante.
- [ ] Quatro estratégias TOWS atualizadas.
- [ ] Prioridades MoSCoW registradas nas Issues relevantes.
- [ ] Funcionalidades adiadas documentadas.
- [ ] Plano de contingência preparado.
- [ ] Materiais da apresentação organizados.
- [ ] Evidências e documentação acessíveis à banca.

## 8. Situação da proposta

Este documento foi elaborado como uma proposta de planejamento da Sprint Final para a atividade AT2 de GAPS.

As decisões apresentadas refletem a análise dos artefatos e das limitações conhecidas do ConectaMente, mas não devem ser interpretadas como aprovação formal da Product Owner.

A incorporação ao planejamento oficial da equipe depende de revisão e decisão dos responsáveis pelo projeto.

## 9. Referências

- README do repositório `gestao` — Análise SWOT e Matriz TOWS.
- Artigo científico do ConectaMente.
- Artefatos do Projeto de Software.
- GitHub Projects — Conectamente.
- Conteúdo da disciplina de Gestão de Agilidade e Projetos de Software (GAPS).## História de Usuário

**Como** integrante da equipe ConectaMente,  
**Desejo** elaborar uma proposta de planejamento estratégico para a Sprint Final,  
**Para** organizar as prioridades, os cortes de escopo e os riscos da apresentação à banca, utilizando os conceitos da disciplina de Gestão de Agilidade e Projetos de Software (GAPS).

## Contexto e Planejamento

O ConectaMente encontra-se na etapa de preparação para a entrega do semestre.

A Análise SWOT e a Matriz TOWS identificam forças, fraquezas, oportunidades e ameaças que devem orientar o planejamento da Sprint Final.

É necessário transformar essas análises em decisões documentadas, utilizando o método MoSCoW, a definição de um fluxo principal demonstrável e estratégias de contingência.

Esta Issue contempla a elaboração de uma **proposta de planejamento**, sujeita à avaliação da Product Owner e da equipe, sem alterar diretamente as decisões registradas na branch `main`.

## Decisões de Escopo

- Definir o fluxo principal previsto para a demonstração à banca.
- Identificar as funcionalidades essenciais para a entrega.
- Classificar as atividades da Sprint Final utilizando MoSCoW.
- Registrar funcionalidades e melhorias propostas para adiamento ao próximo semestre.
- Planejar medidas preventivas contra problemas técnicos na apresentação.
- Definir alternativas de contingência para falhas de hospedagem ou conectividade.
- Manter a proposta em uma branch separada até sua eventual aprovação.

## Regras de Negócio e Critérios de Aceitação

- [ ] O documento deve apresentar o objetivo da Sprint Final.
- [ ] O fluxo principal demonstrável deve estar claramente descrito.
- [ ] As funcionalidades devem ser classificadas por Must Have, Should Have, Could Have e Won't Have, de acordo com o escopo proposto.
- [ ] Os cortes de escopo devem possuir justificativas relacionadas à SWOT e à TOWS.
- [ ] Os principais riscos da apresentação devem ser identificados.
- [ ] Cada risco relevante deve apresentar uma ação preventiva ou de contingência.
- [ ] O planejamento deve diferenciar funcionalidades implementadas, pendentes e adiadas.
- [ ] A proposta deve estar documentada em Markdown e disponível no GitHub para avaliação.

## Definition of Done (DoD)

- [ ] Documento `docs/sprint-final.md` criado no repositório `gestao`.
- [ ] Fluxo principal e decisões de escopo registrados.
- [ ] Priorização MoSCoW documentada.
- [ ] Plano de contingência registrado.
- [ ] Documento revisado quanto à coerência com a SWOT e a TOWS.
- [ ] Commit realizado em branch específica.
- [ ] Pull Request aberto e vinculado à Issue.
- [ ] Proposta disponibilizada à equipe para revisão.

## Observações Técnicas

- **Repositório:** `gestao`
- **Documento:** `docs/sprint-final.md`
- **Branch proposta:** `docs/at2-planejamento-sprint-final`
- **Disciplina:** GAPS
- **Atividade:** AT2 — SWOT e Planejamento da Sprint Final
- **Milestone:** `Sprint Final - Entrega da Banca`
- **Dependência:** consulta à SWOT e à TOWS revisadas na Issue #5.

O documento deve ser identificado como uma proposta elaborada para a AT2. Sua publicação em uma branch e abertura de Pull Request não representam aprovação automática da Product Owner.

## Estimativa

**Story Points: 3**

Estimativa inicial para elaboração, organização e revisão da documentação de planejamento.

## Metadados

- **Type:** Task
- **Priority:** High
- **MoSCoW:** Must Have
- **Status:** In progress
- **Assignee:** responsável pela proposta
- **Milestone:** Sprint Final - Entrega da Banca
