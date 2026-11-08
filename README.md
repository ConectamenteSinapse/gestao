# ConectaMente — Análise SWOT e Matriz TOWS

Jogo sério para auxiliar pessoas com Síndrome de Down nas tarefas diárias.
Projeto Integrador — FATEC Registro (Desenvolvimento de Software Multiplataforma).

## Análise SWOT

A Análise SWOT (*Strengths, Weaknesses, Opportunities, Threats*), também chamada de Matriz FOFA, foi usada como diagnóstico situacional da equipe na reta final do semestre. Os fatores foram separados entre o **ambiente interno**, sob controle da equipe, e o **ambiente externo**, fora do controle direto.

| Dimensão | Natureza | Foco de investigação | Evidências no ConectaMente |
|---|---|---|---|
| **Forças** (*Strengths*) | Interna / Positiva | Habilidades técnicas consolidadas, arquitetura estável e processos eficientes | • API em Node.js e Express organizada em camadas (rotas, controllers, services e models)<br>• Testes automatizados no backend e padronização do código com Prettier e Husky<br>• Segurança com JWT, bcrypt, CORS e autorização por perfil<br>• Proposta embasada em pesquisa científica e no estado da arte |
| **Fraquezas** (*Weaknesses*) | Interna / Negativa | Limitações de plataforma e de acesso | • Jogo disponível apenas para desktop, ainda sem versão mobile |
| **Oportunidades** (*Opportunities*) | Externa / Positiva | Condições externas, ferramentas de mercado e expectativas dos avaliadores | • Hospedagem gratuita em Vercel, Render e MongoDB Atlas<br>• Parcerias com escolas, APAEs e associações de Síndrome de Down<br>• Banca avaliadora focada no fluxo principal do jogo<br>• Alinhamento às ODS 3, 4 e 10 e possibilidade de integração com o CMS |
| **Ameaças** (*Threats*) | Externa / Negativa | Restrições de prazo, instabilidade de plataformas e de infraestrutura | • Data fixa da apresentação para a banca<br>• Plano gratuito do Render coloca a API em repouso após inatividade<br>• Risco de falha de internet no local da apresentação<br>• Exigências da LGPD por envolver dados de crianças |

## Matriz TOWS

A Matriz TOWS cruza os fatores internos e externos da SWOT para gerar ações concretas para a reta final, analisadas na ordem SO, WO, ST e WT.

| Vetor TOWS | Cruzamento analítico | Ação operacional para a reta final |
|---|---|---|
| **Ofensivo** (S×O) | API estável e testada + banca focada no fluxo principal | Demonstrar o fluxo completo de ponta a ponta: cadastro do responsável, criação da criança, partida em um cômodo e relatório de progresso. |
| **Reforço** (W×O) | Jogo disponível apenas para desktop + recursos prontos de CSS responsivo e eventos de toque | Iniciar a adaptação das telas do jogo para dispositivos móveis com media queries e suporte a toque, reaproveitando o padrão responsivo já usado nas telas do responsável. |
| **Confronto** (S×T) | Testes automatizados + instabilidade do plano gratuito do Render | Acessar a API alguns minutos antes da apresentação para tirá-la do repouso e rodar os testes do fluxo principal antes da banca. |
| **Sobrevivência** (W×T) | Jogo disponível apenas para desktop + prazo fixo da banca | Apresentar a versão desktop para a banca e deixar a versão mobile completa, os recursos de áudio e a integração com o CMS para o próximo semestre. |
