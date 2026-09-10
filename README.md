# Vector CANoe & vTESTstudio Training

Repositório público para registrar resultados práticos de exercícios com CANoe e vTESTstudio, com foco em análise CAN/CAN FD, rastreabilidade e automação de testes.

## Escopo

Este repositório contém somente conteúdo produzido durante a prática: anotações, resultados, explicações, evidências próprias e artefatos autorais.

Não são versionados materiais originais de treinamento, instaladores, bancos de dados fornecidos, arquivos `.cfg` originais, slides ou soluções prontas.

## Progresso

### Exercise 1.1 — CANoe Quick Start

Status: em andamento

Resultados já confirmados:

- POWERTRAIN em CAN1
- CAN1 em modo CAN, 500 kbit/s
- BATTERY em CAN2
- CAN2 em ISO CAN FD, 500 kbit/s na fase de arbitragem e 2000 kbit/s na fase de dados
- Trace `T_CAN_All` criada
- coluna `Sender Node` adicionada
- medição iniciada com tráfego CAN/CAN FD visível

Veja os detalhes em [`docs/exercise-01/exercise-1-1.md`](docs/exercise-01/exercise-1-1.md).

## Próximas etapas

- ativar o cenário `Testing (reduced BPC Application)`
- identificar o frame/PDU transmitido por `BPC_00`
- verificar o cycle time
- criar a Graphics Window `G_BMS`
- avançar para projeto de testes no vTESTstudio
