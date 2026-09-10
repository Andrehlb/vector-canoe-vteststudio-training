# Exercise 1.1 — CANoe Quick Start

## Objetivo

Preparar e validar o ambiente inicial no CANoe para observar o tráfego das redes do TrainingCar e identificar os emissores das mensagens.

## Resultados confirmados

### Redes e canais

| Network | CAN Channel | Protocol | Arbitration Bit Rate | Data Rate |
|---|---|---|---:|---:|
| POWERTRAIN | CAN1 | CAN | 500 kbit/s | — |
| BATTERY | CAN2 | ISO CAN FD | 500 kbit/s | 2000 kbit/s |

### Simulation Setup

Foram identificadas as redes `POWERTRAIN` e `BATTERY`.

Na rede BATTERY aparecem o nó `BMS` e os controladores `BPC_00` até `BPC_15`.

### Measurement Setup

Foi criada a Trace Window:

`T_CAN_All`

A coluna `Sender Node` foi adicionada ao layout da Trace.

### Resultado observado

Com a medição iniciada, a `T_CAN_All` passou a exibir tráfego CAN/CAN FD e nós transmissores como `ENGINE`, `BMS`, `BPC_00`, `BPC_01` e outros componentes da simulação.

### Evidência da execução

A captura abaixo registra o CANoe com `Simulation Setup`, `Measurement Setup` e a `T_CAN_All` recebendo tráfego durante a medição.

![Exercise 1.1 - CANoe measurement running](assets/exercise-1-1-result.jpg)

## Próximo passo

Ativar o cenário `Testing (reduced BPC Application)` e usar a `T_CAN_All` para identificar o frame/PDU transmitido por `BPC_00` e seu cycle time.
