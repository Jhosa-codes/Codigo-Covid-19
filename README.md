# Analisador Educacional de Sintomas (COVID-19)

Aplicação de linha de comando em Python que coleta respostas sobre sintomas, calcula uma pontuação heurística e apresenta um gráfico comparativo com frequências estimadas definidas no código.

> **Aviso:** este projeto é um exercício educacional. Não é uma ferramenta médica, não estima risco clínico e não deve ser usado para diagnosticar, descartar COVID-19 ou orientar tratamento. Em caso de sintomas ou preocupação com a saúde, procure um profissional de saúde.

## O que demonstra

- Fluxo de entrada interativo e validação de respostas.
- Regras de pontuação ponderada organizadas em estruturas de dados.
- Visualização com Matplotlib para comparar sintomas informados e valores ilustrativos.
- Separação da lógica de perguntas e geração do gráfico em funções.

## Tecnologias

- Python 3
- Matplotlib

## Como executar

Requer Python 3 instalado.

```bash
git clone https://github.com/Jhosa-codes/Codigo-Covid-19.git
cd Codigo-Covid-19
python -m venv .venv
```

Ative o ambiente virtual:

```bash
# Windows PowerShell
.venv\Scripts\Activate.ps1

# macOS / Linux
source .venv/bin/activate
```

Instale a dependência e execute:

```bash
python -m pip install -r requirements.txt
python covid_test.py
```

Responda `s` ou `n` às perguntas. O programa abre uma janela com o gráfico ao final.

## Como funciona

Cada resposta afirmativa soma o peso associado ao sintoma. A pontuação é comparada com faixas fixas no código para exibir uma mensagem. As frequências usadas no gráfico são valores ilustrativos definidos no próprio script, sem fonte epidemiológica vinculada; não representam dados atuais nem uma probabilidade individual.

## Estrutura

```text
covid_test.py       # Perguntas, pontuação e gráfico
requirements.txt    # Dependências Python
```

## Próximas evoluções

- Separar regras de negócio, interface e visualização.
- Adicionar testes automatizados para validação de entrada e pontuação.
- Documentar a origem de quaisquer dados que venham a ser usados.

## Licença

Nenhuma licença foi identificada neste repositório. Consulte o autor antes de reutilizar ou redistribuir o código.
