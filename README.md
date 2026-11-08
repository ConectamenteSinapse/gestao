# ConectaMente — Análise SWOT e Matriz TOWS

Jogo sério para auxiliar pessoas com Síndrome de Down nas tarefas diárias.  
Projeto Integrador — FATEC Registro (Desenvolvimento de Software Multiplataforma).

## Análise SWOT

A Análise SWOT (*Strengths, Weaknesses, Opportunities, Threats*), também chamada de Matriz FOFA, foi utilizada como diagnóstico situacional da equipe na reta final do semestre.

Os fatores foram separados entre o **ambiente interno**, relacionado às características, capacidades e limitações do projeto, e o **ambiente externo**, relacionado às condições e aos agentes externos à equipe.

A análise considera as funcionalidades documentadas, as melhorias realizadas e as limitações identificadas durante o desenvolvimento do ConectaMente.

| Dimensão | Natureza | Foco de investigação | Evidências no ConectaMente |
|---|---|---|---|
| **Forças** (*Strengths*) | Interna / Positiva | Capacidades técnicas, organização do código, qualidade e fundamentação científica | **S1.** API em Node.js e Express organizada em camadas (rotas, controllers, services e models).<br>**S2.** Testes automatizados no backend e padronização do código com Prettier e Husky.<br>**S3.** Segurança com JWT, bcrypt, CORS e autorização por perfil.<br>**S4.** Proposta embasada em pesquisa científica e no estado da arte.<br>**S5.** Refatoração do `gameController`, com suas funcionalidades distribuídas em 12 controllers, favorecendo a modularização e a manutenção do backend. |
| **Fraquezas** (*Weaknesses*) | Interna / Negativa | Limitações de plataforma, orientação dos usuários e validação de usabilidade | **W1.** Jogo disponível apenas para desktop, ainda sem versão mobile completa.<br>**W2.** Ausência de orientações iniciais no jogo, podendo dificultar a compreensão das atividades no primeiro acesso.<br>**W3.** Ausência de testes de usabilidade com crianças do público-alvo, limitando a avaliação da compreensão das atividades e da adequação das interfaces. |
| **Oportunidades** (*Opportunities*) | Externa / Positiva | Recursos disponíveis, possíveis parcerias e colaboração especializada | **O1.** Disponibilidade de serviços de hospedagem com planos gratuitos, como Vercel, Render e MongoDB Atlas.<br>**O2.** Possibilidade de parcerias com escolas, APAEs e associações de pessoas com Síndrome de Down para divulgação e testes.<br>**O3.** Possibilidade de consultar profissionais envolvidos na pesquisa de personas para orientar melhorias de usabilidade e acessibilidade.<br>**O4.** Alinhamento às ODS 3, 4 e 10, favorecendo a aproximação com iniciativas de educação inclusiva e saúde.<br>**O5.** Possibilidade de alcançar instituições e participantes de diferentes localidades por meio da distribuição do jogo na web. |
| **Ameaças** (*Threats*) | Externa / Negativa | Prazos, dependências de infraestrutura, requisitos legais e disponibilidade de participantes | **T1.** Data fixa da apresentação para a banca, limitando o tempo disponível para desenvolvimento e testes.<br>**T2.** Possibilidade de a API entrar em repouso devido às condições do plano gratuito do Render.<br>**T3.** Risco de indisponibilidade da internet durante a apresentação.<br>**T4.** Exigências da LGPD relacionadas ao tratamento de dados pessoais de crianças.<br>**T5.** Dificuldade de conseguir participantes do público-alvo para testes dentro do prazo do semestre. |

### Considerações sobre a análise

Durante o desenvolvimento, a equipe identificou a necessidade de melhorar a organização de arquivos extensos do backend.

Como ação de melhoria, o `gameController` foi refatorado e suas funcionalidades foram divididas em 12 controllers. Dessa forma, a concentração anterior de responsabilidades não é mantida como uma fraqueza atual.

A ausência de orientações iniciais no jogo permanece como ponto de melhoria. Embora o artigo científico apresente um fluxograma explicando as jornadas da criança e do responsável, esse documento é destinado à compreensão do funcionamento do sistema e não substitui instruções para os jogadores.

O ConectaMente também ainda não passou por testes de usabilidade com crianças do público-alvo. Portanto, a equipe pode apresentar as funcionalidades implementadas e os resultados de testes técnicos realizados, mas não afirmar que a acessibilidade ou a eficácia educacional do jogo já foram validadas com esses usuários.

## Matriz TOWS

A Matriz TOWS cruza os fatores internos e externos identificados na SWOT para transformar o diagnóstico em estratégias concretas de planejamento.

As estratégias foram organizadas em quatro grupos: **SO (Ofensivo), WO (Reforço), ST (Confronto) e WT (Sobrevivência)**.

| Vetor TOWS | Cruzamento analítico | Ação operacional para a reta final |
|---|---|---|
| **Ofensivo (S × O)** | **S1 + S2 + O1 + O5:** arquitetura da API e testes automatizados combinados com hospedagem web e possibilidade de distribuição pelo navegador. | Priorizar a preparação de uma demonstração funcional do fluxo principal do ConectaMente, contemplando cadastro do responsável, vinculação da criança, execução de uma atividade e acompanhamento do progresso, conforme as funcionalidades disponíveis e testadas. |
| **Reforço (W × O)** | **W2 + W3 + O2 + O3:** ausência de orientações iniciais e testes com o público-alvo combinada com oportunidades de colaboração com instituições e profissionais envolvidos na pesquisa de personas. | Consultar profissionais para identificar formas adequadas de apresentar orientações visuais e sonoras, documentando recomendações para implementação e preparando a futura realização de testes com o público-alvo. |
| **Confronto (S × T)** | **S2 + T2 + T3:** testes automatizados do backend combinados com riscos da hospedagem gratuita e indisponibilidade de internet. | Verificar a disponibilidade da API antes da apresentação, executar testes do fluxo principal e preparar uma demonstração gravada como alternativa caso ocorram problemas de conexão, conforme as regras da banca. |
| **Sobrevivência (W × T)** | **W1 + W3 + T1 + T5:** limitação da versão desktop e ausência de validação com o público-alvo combinadas com prazo fixo e dificuldade de recrutamento. | Concentrar a entrega na versão desktop e nas funcionalidades essenciais já desenvolvidas, adiando a adaptação mobile completa, o tutorial visual e sonoro e a validação com crianças do público-alvo para a próxima etapa do projeto. |

### Justificativa das estratégias

As estratégias foram definidas para manter a Sprint Final concentrada na entrega de um fluxo principal demonstrável, evitando a inclusão de funcionalidades que não possam ser concluídas e verificadas dentro do prazo.

A estratégia **SO** busca aproveitar a arquitetura técnica e os recursos de hospedagem para apresentar o funcionamento do jogo.

A estratégia **WO** utiliza oportunidades de colaboração externa para planejar soluções para as limitações de orientação e usabilidade identificadas.

A estratégia **ST** estabelece medidas preventivas e alternativas para reduzir o impacto de falhas técnicas durante a apresentação.

A estratégia **WT** estabelece cortes de escopo, preservando a versão desktop e adiando funcionalidades e validações que dependem de mais tempo e participação externa.

As funcionalidades adiadas permanecem previstas para a evolução do ConectaMente e não são consideradas abandonadas.

## Relação com a Sprint Final e o MoSCoW

A Análise SWOT e a Matriz TOWS orientam a priorização das atividades no GitHub Projects, utilizando o método MoSCoW.

| Prioridade | Diretriz para a Sprint Final |
|---|---|
| **Must Have** | Revisão da documentação estratégica exigida pela AT2, verificação do fluxo principal demonstrável e correção de falhas impeditivas para a entrega. |
| **Should Have** | Melhorias não impeditivas na apresentação e preparação de recomendações de acessibilidade e orientação inicial, conforme a capacidade da equipe. |
| **Could Have** | Ajustes visuais e aperfeiçoamentos complementares que não comprometam os objetivos principais da Sprint. |
| **Won't Have** | Implementação da versão mobile completa, tutorial visual e sonoro completo, integração com CMS e realização da validação com o público-alvo nesta Sprint. |

As atividades adiadas podem permanecer registradas no Backlog para planejamento no próximo semestre.

O planejamento da Sprint Final está associado à Milestone:

**`Sprint Final - Entrega da Banca`**

As Issues devem apresentar responsáveis, prioridades, critérios de aceitação e Definition of Done (DoD), permitindo acompanhar a execução das decisões estratégicas.

## Referências e evidências

- Artigo científico do ConectaMente.
- Artefatos do Projeto de Software.
- Registros e documentação técnica dos repositórios da equipe.
- GitHub Projects da organização ConectamenteSinapse.
- Conteúdo da disciplina Gestão de Agilidade e Projetos de Software (GAPS), FATEC Registro.

Esta análise representa uma revisão da documentação estratégica para a AT2, sujeita à avaliação da Product Owner e da equipe antes de sua incorporação à branch principal.
