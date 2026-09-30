# 💣 Campo Minado

O clássico jogo de minas, com a cara do Windows 98 — jogável direto no navegador, instalável como app (PWA) e com sistema de conquistas estilo Steam.

🔗 **Jogar agora:** https://joaorizzo0112.github.io/campo-minado/

![Demonstração do Campo Minado](demo.gif)

## Funcionalidades

- **Visual clássico do Windows 98**: bevels 3D, LCD vermelho, carinha animada, tudo em pixel font
- **5 dificuldades prontas** (Iniciante → Extraterrestre) **+ dificuldade personalizada** (largura, altura e nº de minas à sua escolha)
- **3 modos de geração do tabuleiro**: totalmente aleatório, início seguro ou pura lógica (gera só tabuleiros resolvíveis sem chute, com um solver embutido)
- **Regras completas do clássico**: bandeira, marcação "?", chord click (clique num número já revelado abre os vizinhos), auto-flag por duplo clique
- **Modo desarmamento**: sobreviva à primeira mina que acertar
- **Botão de dica**: revela uma célula segura com custo de tempo
- **Tutorial jogável**: mini tabuleiro 5×5 que ensina clicando, não só lendo
- **26 conquistas** com pop-up estilo Steam no canto da tela e tela própria para acompanhar o progresso
- **Recorde salvo por dificuldade**, efeitos de vitória (confete) e derrota (tremor de tela + explosão em cascata)
- **Instalável como app** (PWA) no Windows, Android e iOS
- **Site responsivo**, com fundo animado simulando o próprio jogo

## Rodando localmente

Não precisa de build nem dependências — é só abrir o `index.html` no navegador, ou subir a pasta em qualquer servidor estático:

```bash
python3 -m http.server 8000
# depois acesse http://localhost:8000
```

## Estrutura

```
.
├── index.html      # jogo completo (HTML + CSS + JS em um arquivo)
├── manifest.json   # manifest do PWA
├── sw.js           # service worker (cache offline)
├── icons/          # ícones do app em vários tamanhos
└── demo.gif
```

## Feito por

[joaorizzo0112](https://github.com/joaorizzo0112)
