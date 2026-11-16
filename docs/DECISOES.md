# Registro de decisões — GC Games

Este arquivo diferencia decisões explícitas de hipóteses. **Uma sugestão não é uma decisão.**

## Estados
- **Proposta:** em avaliação, sem autorização para implementar como regra.
- **Aprovada:** confirmada explicitamente pelo diretor criativo.
- **Rejeitada:** descartada.
- **Substituída:** decisão revogada por outra, com referência.

## Decisões aprovadas
| ID | Data | Área | Decisão | Status |
|---|---|---|---|---|
| DEC-001 | 2026-11-16 | Governança | O criador dirige narrativa e acontecimentos; apoio técnico não decide por ele | Aprovada |
| DEC-002 | 2026-11-16 | Processo | Priorizar concepção e documentação antes de implementar multiplayer | Aprovada |
| DEC-003 | 2026-11-16 | Organização | Manter repositório GitHub `AllanNyko/gc-games` para organizar o projeto | Aprovada |

## Ideias discutidas — não aprovadas como especificação final
| ID | Assunto | Hipótese | Status |
|---|---|---|---|
| PROP-001 | Defesa | Defender uma casa, igreja ou outro ponto | Proposta |
| PROP-002 | Inimigos | Hordas de criaturas monstruosas | Proposta |
| PROP-003 | Vitória | Resistir até o término de um timer e avançar | Proposta |
| PROP-004 | Câmera | Visão elevada ao andar e sobre o ombro ao mirar | Proposta para protótipo |
| PROP-005 | Tecnologia | Godot/GDScript para Android | Em avaliação |
| PROP-006 | Cooperação | Dois celulares Android, cada criança no seu | Intenção de produto |

## Procedimento
1. Documentar contexto e alternativas usando [o template](decisoes/TEMPLATE.md).
2. Discutir impactos criativos, de jogabilidade e técnicos.
3. Solicitar decisão do criador, sem presumir sua aprovação.
4. Atualizar este registro, com data, status e justificativa.


## Decisões adicionais — 2026-11-16
| ID | Área | Decisão | Status |
|---|---|---|---|
| DEC-004 | Modos | Existirão Modo História e Modo Missões; este último permite partidas rápidas sem seguir a campanha | Aprovada |
| DEC-005 | Narrativa | Escolhas explícitas e consequências de ações/omissões influenciarão eventos futuros; pessoas resgatadas podem reaparecer | Aprovada |
| MIS-001 | Preparação | Antes de cada missão, o usuário terá 15 segundos para selecionar o que levar | Aprovada |
| MIS-002 | Preparação | Se o usuário não selecionar, receberá um equipamento padrão | Aprovada |
| INV-001 | Coleta | Durante missões, jogadores podem obter e transportar itens encontrados | Aprovada |
| INV-002 | Mochila | Transporte limitado pela capacidade da mochila | Aprovada |
| INV-003 | Expiração | Política de validade/expiração de itens ainda não definida | Pendente — não implementar |

**Nota:** a proposta de expiração semanal foi expressamente adiada pelo diretor criativo. Não assumir reset, calendário, duração ou exceções.

**Pontos ainda sem aprovação:** dimensão da mochila, conteúdo do equipamento padrão, quais itens se mantêm após o reset, horário e fuso da expiração, condições de retenção de itens após derrota e integração dos inventários entre modos.
