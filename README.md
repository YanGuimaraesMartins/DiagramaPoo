# DiagramaPoo

### Exemplo de Diagrama UML (Mermaid)
```mermaid
classDiagram
    interface ReprodutorMusical {
        public void tocar();
        public void pausar();
        public selecionarMusica(String musica); 
    }

    interface AparelhoTelefonico {
        public void ligar(String numero);
        public void atender(); 
        public void iniciarCorreioVoz();
    }

    interface NavegadorInternet {
        public void exibirPagina(String url);
        public void adicionarNovaAba();
        public void atualizarPagina();
    }

    class iPhone implements
ReprodutorMusical, AparelhoTelefonico, NavegadorInternet {
        public void tocar();
        public void pausar();
        public selecionarMusica(String musica);
        public void ligar(String numero);
        public void atender(); 
        public void iniciarCorreioVoz();
        public void exibirPagina(String url);
        public void adicionarNovaAba();
        public void atualizarPagina();
    }

    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorInternet
```
