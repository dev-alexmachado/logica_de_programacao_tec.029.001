# Lista de atividades

## Atividade 01

Crie o código em Python do fluxograma abaixo:
~~~mermaid
flowchart TD
    A([Início])
    B@{ shape: manual-input, label: "str nome\nstr email\nstr cpf\nstr telefone\nint idade\nfloat altura" }
    C@{ shape: curv-trap, label: "Nome: &nome\nE-mail: &email\nCPF: &cpf\nTelefone: &telefone\nIdade: &idade anos\nAltura: &altura metros" }
    D([Fim])

    A --> B
    B --> C
    C --> D
~~~

## Atividade 02

Crie o código em Python do fluxograma abaixo:
~~~mermaid
flowchart TD
    A([Início])
    B@{ shape: manual-input, label: "int n1" }
    C@{ shape: manual-input, label: "int n2" }
    D[soma = n1 + n2]
    E[subtracao = n1 - n2]
    F[multiplicacao = n1 * n2]
    G[divisao = n1 / n2]
    H[resto = n1 % n2]
    I@{ shape: curv-trap, label: "Soma: &soma\nSubtração: &subtracao\nMultiplicação: &subtracao\nDivisão: &divisao\nResto da divisão: &resto" }
    J([Fim])

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G
    G --> H
    H --> I
    I --> J
~~~

## Atividade 03

Crie o código em Python do fluxograma abaixo:
~~~mermaid
flowchart TD
    A([Início])
    B@{ shape: manual-input, label: "str nome" }
    C@{ shape: manual-input, label: "int idade" }
    D{idade >= 18}
    E@{ shape: curv-trap, label: "&nome é maior de idade" }
    F@{ shape: curv-trap, label: "&nome é menor de idade" }
    G([Fim])

    A --> B --> C --> D
    D -- Sim --> E
    D -- Não --> F
    E --> G
    F --> G
~~~

## Atividade 04

Crie o código em Python do fluxograma abaixo:
~~~mermaid
flowchart TD
    A([Início])
    B@{ shape: manual-input, label: "float massa" }
    C@{ shape: manual-input, label: "float altura" }
    D{massa <= 140}
    E{altura >= 1,15}
    F@{ shape: curv-trap, label: "Entrada do usuário negada." }
    G@{ shape: curv-trap, label: "Entrada do usuário permitida." }
    H([Fim])

    A --> B --> C --> D
    D -- Sim --> E
    D -- Não --> F
    E -- Sim --> G
    E -- Não --> F
    F --> H
    G --> H
~~~

## Atividade 05

Crie o código em Python do fluxograma abaixo:
~~~mermaid
flowchart TD
    A([Início])
    B@{ shape: manual-input, label: "str nome" }
    C@{ shape: manual-input, label: "int nota1" }
    D@{ shape: manual-input, label: "int nota2" }
    E["media = (nota1 + nota2)/2"]
    F@{ shape: curv-trap, label: "Média: &media" }
    G{media >= 7}
    H@{ shape: curv-trap, label: "&nome está aprovado" }
    I{media >= 5}
    J@{ shape: curv-trap, label: "&nome está de recuperação" }
    K@{ shape: curv-trap, label: "&nome reprovado" }
    L([Fim])

    A --> B --> C --> D --> E --> F --> G
    G -- Sim --> H
    G -- Não --> I
    I -- Sim --> J
    I -- Não --> K
    H --> L
    J --> L
    K --> L
~~~
