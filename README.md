# Sistema de Controle Logístico Lunar (SCLL)

Projeto desenvolvido pela **Equipe Lua** para a atividade de **Mission Control**, com o tema **Foguete e Logística**.

## Sobre o projeto

O **Sistema de Controle Logístico Lunar (SCLL)** foi desenvolvido para apoiar o **Centro de Controle** na decisão sobre missões de logística lunar. O sistema avalia a combinação de **veículo, carga e janela/local**, considerando a viabilidade de combustível, bateria e o nível de risco antes de autorizar uma operação.

Foram utilizadas as bases:

- `veiculos_logisticos`
- `cargas`
- `janelas_operacao`
- `telemetria_pouso`
- `locais_pouso_apollo`

Esses dados permitem analisar a **capacidade da frota, a prioridade das cargas, o risco das janelas de operação, a saúde dos veículos durante o pouso e os locais históricos de referência**.

## O sistema analisa

- **Número de veículos disponíveis**
- **Carga de maior prioridade**
- **Janela de operação mais segura**
- **Status da telemetria por temperatura do motor e vibração**
- **Classificação geral de risco da missão**

Os status de telemetria são:

- `NORMAL`
- `ALERTA`
- `CRÍTICO`

A missão pode ser classificada como:

- `NORMAL`
- `ALERTA`
- `CRÍTICA`
- `MISSÃO CONDENADA`

## Programas

O projeto possui **dois programas principais**:

### `programa_01_monitoramento.py`

Monitora o estado geral da operação, considerando **frota, cargas, janelas de lançamento e telemetria**, gerando um diagnóstico da base lunar.

### `programa_02_simulador.py`

Permite que o usuário escolha um **veículo, uma carga e um local** para simular uma missão específica.

A partir dessas escolhas, o sistema aplica as **regras de risco** e apresenta uma classificação e recomendação para o cenário.

## Decisão esperada

Ao final da simulação, o sistema apresenta uma **recomendação** indicando se a missão:

- Pode prosseguir normalmente;
- Exige atenção;
- É arriscada;
- Não deve ser autorizada.

## Equipe

**Equipe Lua — Turma 1 CCPJ**

| Integrante | RM |
|---|---|
| André Debiazzi | RM569062 |
| Kaique da Silva Assis | RM572718 |
| Vinicius Cristal | RM572049 |
| Maria Eduarda Rocha Benjamim | RM570554 |
| Pedro Henrique Neves | RM571382 |
| Akin Alexandre Mendes Martins | RM572773 |
