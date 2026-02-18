```markdown
# 🎨 GIF Animator em Go

Este projeto gera **GIFs animados de curvas de Lissajous** utilizando apenas a biblioteca padrão do Go.  
É um exemplo clássico que mostra como o Go pode manipular imagens e criar animações sem dependências externas.

---

## 🚀 Como funciona
O programa:
1. Define uma paleta de cores (ex.: vermelho e azul).
2. Calcula curvas de Lissajous usando funções trigonométricas.
3. Gera múltiplos frames (`nframes`) com pequenas variações de fase.
4. Codifica todos os frames em um GIF animado (`out.gif`).

---

## 📂 Estrutura do projeto
```
.
├── main.go   # Código principal
├── go.mod    # Módulo Go
└── out.gif   # GIF gerado
```

---

## ▶️ Executando

### 1. Inicializar módulo
```bash
go mod init gif-animator
go mod tidy
```

### 2. Rodar o programa
```bash
go run main.go
```

Isso gera o arquivo `out.gif` na pasta atual.

### 3. Visualizar
Abra `out.gif` em qualquer navegador ou visualizador de imagens.

---

## ⚙️ Configurações principais
No código, você pode alterar:

- `cycles` → número de ciclos da curva.
- `size` → tamanho da imagem.
- `nframes` → quantidade de frames da animação.
- `delay` → tempo entre frames.
- `palette` → cores usadas (ex.: `color.RGBA{255,0,0,255}` para vermelho).

---

## 🖌️ Exemplo de paleta personalizada
```go
var palette = []color.Color{
    color.RGBA{255, 0, 0, 255},   // vermelho
    color.RGBA{0, 0, 255, 255},   // azul
}
```

---

## 📦 Dependências
Nenhuma dependência externa.  
O projeto usa apenas a **biblioteca padrão do Go** (`image`, `gif`, `math`, etc.).

---

## ✨ Resultado
O programa gera um GIF animado interativo com padrões geométricos que mudam a cada execução, pois a frequência é sorteada aleatoriamente.

---

## 📜 Licença
Este projeto é livre para estudo e uso pessoal.
```

---

👉 Esse README já explica como rodar, configurar e visualizar o GIF. Quer que eu adicione também uma seção mostrando como transformar o programa em um **servidor HTTP** que serve o GIF direto no navegador (`localhost:8080`)?

