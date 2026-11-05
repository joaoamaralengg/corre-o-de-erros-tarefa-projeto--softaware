# Correção de erros — Timeline

Este repositório guarda quatro atividades feitas para o projeto [GabrielaJusto/Timeline](https://github.com/GabrielaJusto/Timeline).

**Ele não funciona sozinho.** Cada pasta tem apenas os arquivos alterados naquela atividade, sem o `manage.py` e o restante do projeto. Para funcionar, os arquivos precisam ser colocados no repositório original.

## Atividades

| Pasta | O que faz |
|---|---|
| `marcar-atividade-como-concluida` | Permite concluir e reabrir atividades e calcula o progresso |
| `criar-pagina-de-notificacoes` | Liga a página de notificações, com rotas, avisos e item no menu |
| `setas-de-troca-de-semana` | Faz as setas da agenda semanal funcionarem |
| `datas-em-portugues-e-fuso-de-brasilia` | Coloca o projeto em português e no fuso de Brasília |

## Como usar

1. Clone o repositório original e volte para o commit usado como base:

   ```bash
   git clone https://github.com/GabrielaJusto/Timeline.git
   cd Timeline
   git checkout c845cbf
   ```

2. Copie o conteúdo da pasta da atividade para a raiz do projeto, substituindo os arquivos existentes:

   ```bash
   cp -R ../corre-o-de-erros-tarefa-projeto--softaware/setas-de-troca-de-semana/. .
   ```

   Troque `setas-de-troca-de-semana` pelo nome da atividade desejada. O comando considera que os dois repositórios estão na mesma pasta.

3. Rode os testes e inicie o projeto:

   ```bash
   python manage.py test core
   python manage.py runserver
   ```

## Atenção

- **Uma atividade por vez:** cada atividade foi feita em uma cópia separada do projeto, e várias substituem os mesmos arquivos, como `core/views.py` e `core/tests.py`. Copiar uma por cima da outra apaga as alterações da anterior.
- **Versão do Python:** `setas-de-troca-de-semana` exige Python 3.12 ou mais recente.
