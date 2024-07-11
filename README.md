# DiagramaPoo

### Exemplo de Diagrama UML (Mermaid)
```mermaid
classDiagram
    interface ReprodutorMusical {
        + tocar()
        + pausar()
        + selecionarMusica(String musica)
    }

    interface AparelhoTelefonico {
        + ligar(String numero)
        + atender()
        + iniciarCorreioVoz()
    }

    interface NavegadorInternet {
        + exibirPagina(String url)
        + adicionarNovaAba()
        + atualizarPagina()
    }

    class iPhone {
        + tocar()
        + pausar()
        + selecionarMusica(String musica)
        + ligar(String numero)
        + atender()
        + iniciarCorreioVoz()
        + exibirPagina(String url)
        + adicionarNovaAba()
        + atualizarPagina()
    }

    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorInternet

```
