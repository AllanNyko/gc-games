# GC Games — Game Design Document (GDD)

**Versão:** 0.1 (concepção)  
**Data:** 2026-11-16  
**Estado:** documento de trabalho; nenhuma mecânica descrita como hipótese está aprovada automaticamente.

## 1. Propósito
Conceber um jogo para Android, pensado inicialmente para uma criança de 6 anos e seu primo jogarem em aparelhos separados. A experiência, história e acontecimentos são definidos pelo criador do projeto. O apoio técnico pode propor soluções, mas não define narrativa nem escopo unilateralmente.

## 2. Conceito em discussão
Uma ou duas pessoas defendem um ponto (por exemplo, casa ou igreja) contra uma horda de criaturas. A proposta inicial é sobreviver durante um tempo determinado para avançar de nível. Trata-se de **ideia exploratória**, não de regras fechadas.

### Referências
- *Resident Evil*: câmera em terceira pessoa e mira sobre o ombro (referência de enquadramento, não de conteúdo violento).
- *Sifu*: sensação de exploração, combate e progressão (referência de qualidade e experiência, não de cópia).
- Jogos de defesa contra hordas: inspiração para estrutura de partidas.

## 3. Câmera — hipótese central para prototipagem
- **Movimentação/exploração:** câmera elevada, com personagem visível e maior leitura do cenário.
- **Mirar/disparar:** câmera aproxima-se suavemente para posição sobre o ombro.
- **Ao encerrar a mira:** retorno à perspectiva elevada é uma possibilidade; comportamento definitivo pendente.
- Considerar oclusão de paredes, rotação do personagem, sensibilidade, recuo visual e legibilidade em tela pequena.

## 4. Mecânicas em estudo
| Tema | Possibilidade | Estado |
|---|---|---|
| Objetivo | Defender local, sobreviver ou ambos | Aberto |
| Ondas | Criaturas surgem em grupos ou continuamente | Aberto |
| Timer | Resistir até o fim do tempo | Aberto |
| Combate | Mira e disparo com câmera sobre o ombro | Em discussão |
| Progressão | Níveis, equipamentos, habilidades ou novos locais | Aberto |
| Exploração | Circular pelo cenário, usar objetos e encontrar recursos | Aberto |
| Cooperação | Um ou dois jogadores, celulares Android separados | Intenção |
| Inimigos | Tipo, comportamento, aparência e intensidade | Aberto |
| Enredo | Mundo, personagens, causas e acontecimentos | Exclusivo do diretor criativo |

## 5. Faixa etária e experiência
O primeiro público pretendido tem cerca de 6 anos. Antes de definir o visual dos monstros, intensidade do combate, sustos, dificuldade e controles, avaliar adequação etária. Preferir protótipos com violência não gráfica e mecanismos de acessibilidade.

## 6. Plataforma e arquitetura em avaliação
- **Destino:** Android.
- **Engine candidata:** Godot, com GDScript.
- **Tipo:** 3D em terceira pessoa, com duas perspectivas dinâmicas.
- **Multiplayer:** objetivo futuro; não fixar topologia, servidor ou sincronização agora.
- **Protótipo:** validar primeiro movimentação, mudança de câmera e uma interação de mira/disparo com recursos provisórios.

## 7. Recursos de desenvolvimento conhecidos
- Dell Inspiron 3583, i7-8565U, Intel UHD 620, 16 GB RAM, SSD SATA 2 TB e NVMe 256 GB.
- Outro notebook Ubuntu com i5-1035G1, ~8 GB RAM reconhecidos, Intel Iris Plus G1 e partição do sistema quase cheia no último diagnóstico.
- ROG Ally X disponível em outro momento, candidato ao desenvolvimento 3D principal.
- **Atenção:** a capacidade dos computadores de desenvolvimento não representa o desempenho dos aparelhos Android de destino.

## 8. Itens deliberadamente não definidos
Título final; universo; personagens; enredo; locais; armas; estética e intensidade dos monstros; condição de vitória/derrota; quantidade de hordas; duração; sistema de evolução; economia; monetização; controles finais; arquitetura de rede.

## 9. Critério de validação de protótipo (sugestão, não aprovação)
1. Personagem se movimenta em uma arena simples.
2. Visão elevada permite explorar e ler ameaças.
3. Ao mirar, câmera transita ao ombro sem travar controles.
4. Disparo tem direção correta e resposta visual clara.
5. Teste no Android confirma legibilidade e FPS aceitáveis.

## 10. Perguntas criativas pendentes
- A defesa envolve impedir dano à estrutura, sobreviver ou ambos?
- A fase termina quando o timer zera, quando a horda acaba ou sob outra condição?
- Qual nível de tensão/terror é desejado para as crianças?
- Os locais mudam a cada rodada?
- Como seria a evolução entre partidas?
- O retorno da câmera após a mira deve ser automático ou configurável?

## 11. Governança
Consulte [DECISOES.md](DECISOES.md). Só promover propostas a decisões mediante manifestação explícita do criador. Registrar mudanças e substituições, não reescrever a história do projeto como se sempre tivesse sido assim.


## 12. Modos e decisões de partida (atualização 2026-11-16)
- **Modo História:** exploração, resgate e consequências persistentes derivadas de escolhas explícitas, ações e omissões. Sobreviventes resgatados podem reaparecer futuramente, conforme acontecimentos ainda definidos pelo diretor criativo.
- **Modo Missões:** partidas avulsas, sem obrigação de seguir a história, destinadas inclusive a sessões rápidas entre amigos.
- **Pré-missão:** período de **15 segundos** para escolher o equipamento que o jogador levará.
- **Sem escolha:** aplicar automaticamente um **equipamento padrão**, cuja composição permanece indefinida.
- **Coleta:** jogadores podem encontrar e levar itens obtidos durante as missões, condicionados ao **espaço disponível na mochila**.
- **Expiração:** itens obtidos têm renovação/expiração **toda segunda-feira**, conforme instrução do criador. A expressão “validade de uma semana” precisa ser conciliada com reset semanal: até confirmação, o calendário da segunda-feira é a regra operacional registrada, não sete dias individuais contados por item.

### Questões em aberto (não presumir)
- Horário e fuso do reset de segunda-feira; como tratar missões iniciadas antes da virada.
- Se o reset abrange todos os itens coletados, inclusive os equipados, ou exceções.
- Quais itens básicos persistem para compor o equipamento padrão.
- Capacidade da mochila (slots, peso, volume) e como itens ocupam espaço.
- Se itens coletados são preservados ao abandonar ou perder uma missão.
- Compartilhamento ou independência dos inventários de Modo História e Modo Missões.
- Equipamentos disponíveis para escolher nos 15 segundos e comportamento dos demais jogadores.
