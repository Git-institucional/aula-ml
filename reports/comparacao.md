# Comparação entre r1 e r2

## Alteração feita

Rótulo do chamado 006 ("bloqueio de acesso") corrigido de `comum` para `urgente`.
A partição de treino e teste (`data/split.csv`) não mudou.

## Métricas (mesma partição de teste, 4 exemplos)

| Modelo | Dataset | Acurácia | Recall urgente | Recall comum |
|--------|---------|----------|----------------|--------------|
| r1     | v1      | 3/4      | 1/2            | 2/2          |
| r2     | v2      | 4/4      | 2/2            | 2/2          |

## Hashes verificados no clone limpo (modelo-r1)

- Commit: PREENCHER_SHA_DO_COMMIT
- data/chamados.csv: PREENCHER_HASH
- data/split.csv: PREENCHER_HASH
- models/model.json: PREENCHER_HASH

## Decisão

Aceitar r2. O recall de urgentes melhorou sem reduzir o recall de comuns, com a mesma partição de teste.
O conjunto de teste é pequeno, então o resultado vale como demonstração neste exercício.
