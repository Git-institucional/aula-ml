# aula-ml

Versionamento de dados e modelos com Git e DVC (CK0444, Atividade Prática 07).

## Pré-requisitos

- Git
- Python 3.10 ou superior
- DVC 3 (`pipx install 'dvc>=3,<4'`)

## Armazenamento DVC

O remote padrão `storage` aponta para a pasta irmã `../dvc-storage`.
Ela precisa existir ao lado deste repositório e conter os artefatos enviados com `dvc push`.
Confira com `dvc remote list`.

## Restaurar uma versão

```bash
git clone <URL_DO_REPOSITORIO> aula-ml-restauracao
cd aula-ml-restauracao
git switch --detach modelo-r1   # ou dados-v1, dados-v2, modelo-r2
dvc pull
```

## Tags

- `dados-v1`: dataset inicial (erro de rótulo no ID 006)
- `modelo-r1`: modelo treinado com `chamados-v1`
- `dados-v2`: dataset com o rótulo corrigido
- `modelo-r2`: modelo treinado com `chamados-v2`
