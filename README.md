# DiagramaPoo

### Exemplo de Diagrama UML (Mermaid)
```mermaid
classDiagram
    interface ReprodutorMusical {
        +tocar() : void
        +pausar() : void
        +selecionarMusica(String musica) : String
    }

    interface AparelhoTelefonico {
        +ligar(String numero) : void
        +atender() : void
        +iniciarCorreioVoz() : void
    }

    interface NavegadorInternet {
        +exibirPagina(String url): void
        +adicionarNovaAba(): void
        +atualizarPagina(): void
    }

    class iPhone implements
ReprodutorMusical, AparelhoTelefonico, NavegadorInternet {
        +tocar() : void
        +pausar() : void
        +selecionarMusica(String musica) : String
        +ligar(String numero) : void
        +atender() : void
        +iniciarCorreioVoz() : void
        +exibirPagina(String url): void
        +adicionarNovaAba(): void
        +atualizarPagina(): void
    }

    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorInternet
```
