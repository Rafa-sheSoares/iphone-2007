# iPhone 2007 - Diagrama UML e Implementação

## Diagrama UML

```mermaid
classDiagram
    class ReprodutorMusical {
        <<interface>>
        + tocar(): void
        + pausar(): void
        + selecionarMusica(musica: String): void
    }

    class AparelhoTelefonico {
        <<interface>>
        + ligar(numero: String): void
        + atender(): void
        + iniciarCorreioVoz(): void
    }

    class NavegadorInternet {
        <<interface>>
        + exibirPagina(url: String): void
        + adicionarNovaAba(): void
        + atualizarPagina(): void
    }

    class iPhone {
        - reprodutorMusical: ReprodutorMusical
        - aparelhoTelefonico: AparelhoTelefonico
        - navegadorInternet: NavegadorInternet
        + iPhone()
    }

    iPhone ..|> ReprodutorMusical
    iPhone ..|> AparelhoTelefonico
    iPhone ..|> NavegadorInternet
```

## Descrição

Este projeto representa a modelagem das funcionalidades do iPhone original de 2007, incluindo:
- Reprodutor Musical
- Aparelho Telefônico
- Navegador de Internet

## Como Executar

1. Compile os arquivos Java
2. Execute a classe `iPhone`

## Tecnologias

- Java
- UML
- Mermaid para diagrama