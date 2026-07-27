<h2 align="center">Prismo</h2>
<p align="center">
   <b>Realize seus sonhos através de um prisma</b>
</p>


### Sobre o projeto

Há algum tempo, as interfaces complicadas de aplicativos modernos de desenho me fizeram pensar bastante a respeito de um sentimento que vem se esgueirando no meu subconsciente.

Acontece que essa complicação desnecessária, que acaba por estender a curva de aprendizado, apenas me faz afastar cada vez mais de um ramo pelo qual sou apaixonado e sempre tive curiosidade e vontade de aprender mais.

E sim, eu concordo que todas essas ferramentas são extremamente poderosas, mas eu penso em um iniciante no mundo da arte, assim como eu sou.

Ter que aprender tudo o que diz respeito à arte digital e, além disso, escolher um software para chamar de seu é realmente um desafio e tanto.

E então eu pensei nesse programa. A princípio, imaginei refazer o Paint para uma versão mais moderna (que tenha layers), porque eu adoro usar o Paint e sinto que ele comete apenas um pecado: não poder usar camadas. Sim, eu sou louco.

O legal é que ter um programa de rabiscos que seja meu é uma tarefa que vai me ensinar MUITA coisa, e quem me conhece há algum tempo sabe que eu sou `A P A I X O N A D O` por aprender algo novo! Então pensei em desenvolver o projeto completo!

E quem sabe, ao longo do projeto, tirar outras ideias para esse programa do papel.

Meu intuito é catalogar todo o desenvolvimento. Eu quero desenvolver um programa de desenho que seja de fácil acesso, open source, que seja extremamente poderoso, para que enfim, aquela frase de "qualquer pessoa pode aprender a desenhar" se torne verdadeira!

Não quero criar apenas um papel digital. Quero criar um `prisma` que, ao olhar através dele, permita enxergar minhas ideias mais loucas.

Então, acompanhe-me em [meu canal no YouTube](https://www.youtube.com/@mitchzito) para saber mais sobre esse projeto!


### Tecnologias utilizadas

| Categoria             | Tecnologia                                          |
|-----------------------|-----------------------------------------------------|
| **Linguagem**         | Python 3.10+                                        |
| **Interface Gráfica** | PySide6 (Qt for Python)                             |

### Recursos Planejados

#### Motor Gráfico
* Renderização via `QGraphicsView` / `QGraphicsScene`
* Manipulação de pixels com `QImage`

#### Funcionalidades
* Sistema de camadas não-destrutivo
* Histórico de ações (Undo/Redo)
* Exportação de imagens em múltiplos formatos

### Funcionalidades

#### Implementadas

* [X] Estrutura inicial do projeto
* [ ] Janela principal
* [ ] Sistema base de telas
* [ ] Gerenciamento de assets

#### Em desenvolvimento

* [ ] Canvas de desenho
* [ ] Ferramenta lápis
* [ ] Borracha
* [ ] Seleção de cores
* [ ] Controle de camadas
* [ ] Undo / Redo
* [ ] Salvamento de projetos

#### Futuras

* [ ] Sistema de plugins
* [ ] Filtros de imagem
* [ ] Ferramentas vetoriais
* [ ] Atalhos personalizáveis
* [ ] Suporte a mesa digitalizadora
* [ ] Formato próprio de arquivo PRISMO

### Estrutura do projeto

```
PRISMO/
│
├── main.py                 # Inicialização do programa
│
├── core/                   # Componentes fundamentais
│   ├── qt.py               # Imports do PySide6
│   ├── config.py           # Configurações globais
│   └── paths.py            # Gerenciamento de caminhos
│
├── ui/                     # Interface gráfica
│   ├── base_window.py      # Janela base
│   │
│   ├── main_window/        # Tela inicial
│   │
│   ├── canvas_window/      # Editor de desenho
│   │
│   └── widgets/            # Componentes reutilizáveis
│
├── engine/                 # Motor do aplicativo
│   ├── canvas.py           # Manipulação do desenho
│   ├── layer.py            # Sistema de camadas
│   ├── tools.py            # Ferramentas
│   └── history.py          # Histórico de ações
│
├── assets/                 # Recursos visuais
│   ├── icons/
│   └── images/
│
└── storage/                # Dados do usuário
    ├── projects/
    └── exports/
```

## Instalação

### Requisitos

* Python 3.10 ou superior
* pip
* Ambiente virtual recomendado

### Criando ambiente virtual

Windows:

```bash
   python -m venv venv
```

Ativar:

```bash
   venv\Scripts\activate
```

Linux/macOS:

```bash
   source venv/bin/activate
```

### Instalando dependências

```bash
   pip install -r requirements.txt
```

## Executando

Execute:

```bash
   python main.py
```


## Desenvolvimento

Durante o desenvolvimento, recomenda-se:

* Manter a lógica separada da interface.
* Evitar colocar regras de negócio dentro dos widgets.
* Utilizar o diretório `engine` para funcionalidades do editor.
* Utilizar o diretório `ui` apenas para componentes visuais.

Arquitetura:

```
      ┌───────────┐
      │ Interface │ 
      └───────────┘
           ┃
           ┃
           ▼
      ┌───────────┐
      │  Engine   │ 
      └───────────┘
           ┃
           ┃
           ▼
      ┌───────────┐
      │   Dados   │ 
      └───────────┘
```


<p align="center">
  <img src="https://readme-typing-svg.demolab.com/?lines=O+PRISMO+n%C3%A3o+%C3%A9+apenas+um+papel+digital.;Ele+%C3%A9+um+prisma+que;ao+olhar+atrav%C3%A9s+dele,+permite+que+voc%C3%AA;enxergue+suas+ideias+mais+loucas.&font=Fira%20Code&center=true&color=64F58E&width=1000&height=50&duration=4000&pause=1000" alt="PRISMO">
</p>

## Licença

Projeto pessoal desenvolvido para uso pessoal e portfólio. `PRISMO © 2026`
