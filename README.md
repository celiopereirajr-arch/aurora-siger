# Ignition Zero: O Início da Aurora
## Relatório Operacional de Pré-Decolagem

Projeto acadêmico da FIAP, do curso de Ciência da Computação (Online), que simula um sistema de verificação de pré-decolagem para uma nave fictícia, a Aurora Siger. O objetivo é analisar dados de telemetria e decidir, de forma automatizada, se a nave está apta para o lançamento ("PRONTO PARA DECOLAR") ou se a decolagem deve ser abortada ("DECOLAGEM ABORTADA").

O projeto integra:

- Interpretação e organização de dados de telemetria
- Um algoritmo de verificação determinístico (fluxograma + pseudocódigo + implementação em Python)
- Uma análise energética (autonomia estimada da nave)
- Uma análise assistida por IA, complementar às verificações determinísticas
- Uma reflexão crítica sobre ética, impacto social e sustentabilidade tecnológica

## Estrutura do repositório

```
├── projeto/                        # Arquivos do projeto
│   ├── ignition_zero.ipynb         # Notebook com todo o desenvolvimento
│   └── fluxograma-verificacao.png  # Fluxograma do algoritmo de verificação
└── README.md                       # Este arquivo            
```

## Como executar

1. Baixe ou clone este repositório, mantendo o notebook e a imagem `fluxograma-verificacao.png` na `projeto/`.
2. Abra o arquivo `projeto/ignition_zero.ipynb` no [Google Colab](https://colab.research.google.com/) ou em um ambiente Jupyter.
3. Se for usar o Colab, faça upload de `fluxograma-verificacao.png` na sessão (ícone de pasta → upload) antes de rodar a célula responsável por exibi-la. Sem isso, a célula simplesmente exibe um aviso informando onde encontrar a figura, sem quebrar a execução das demais células.
4. Rode as células em sequência (Ambiente de execução → Executar tudo). Não há dependências externas; o projeto utiliza apenas a biblioteca padrão do Python.

## Resultados da execução

**Algoritmo de verificação: Cenário Principal (dados da seção 5.1):**

```
=============================================
RELATÓRIO DE VERIFICAÇÃO — PRÉ-DECOLAGEM
=============================================

STATUS: DECOLAGEM ABORTADA

Motivo(s):
 - Temperatura externa: -280 fora da faixa segura (-270 a -100)
 - Pressão dos tanques: 320 fora da faixa segura (150 a 300)
=============================================
```

**Algoritmo de verificação: Cenário de Contraste (valores totalmente dentro da faixa):**

```
=============================================
RELATÓRIO DE VERIFICAÇÃO — PRÉ-DECOLAGEM
=============================================

STATUS: PRONTO PARA DECOLAR

Todas as verificações foram aprovadas.
=============================================
```

**Análise energética:**

```
Energia disponível: 850.0 kWh
Perdas energéticas: 68.0 kWh
Energia líquida: 782.0 kWh
Energia restante após decolagem: 562.0 kWh
Autonomia estimada: 5.62 horas
```

## Tecnologias utilizadas

- Python 3 (biblioteca padrão apenas. Sem dependências externas)

## Autor

Célio Carlos Pereira Junior (RM: 574595)
FIAP: Ciência da Computação (Online)
