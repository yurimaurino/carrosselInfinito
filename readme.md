# 🎠 Carrossel Infinito

Um componente de carrossel infinito com animação CSS pura, suporte a duas faixas (normal e reversa), efeito de pausa no hover.

---

## 📁 Estrutura do Projeto

```
projeto/
├── index.html
├── styles.css
└── images/
    ├── portfolio3.png
    ├── item1-1.png
    ├── item1-2.png
    │   ...
    ├── item1-10.png
    ├── item2-1.png
    │   ...
    └── item2-9.png
```

---

## 🚀 Como usar

1. Clone ou baixe o repositório
2. Adicione suas imagens na pasta `images/`
3. Abra o `index.html` no navegador — nenhuma dependência ou build necessário

---

## ⚙️ Como funciona

O carrossel usa `position: absolute` e animações CSS com `@keyframes` para mover cada item da direita para a esquerda (ou o inverso). O espaçamento entre os itens é controlado pelo `animation-delay` de cada item.

### Variáveis CSS

Cada `.container` aceita três variáveis customizadas via `style` inline:

| Variável | Descrição | Exemplo |
|---|---|---|
| `--width` | Largura de cada item | `100px` |
| `--height` | Altura de cada item | `50px` |
| `--quantity` | Número de itens no carrossel | `10` |

Cada `.item` aceita uma variável:

| Variável | Descrição | Exemplo |
|---|---|---|
| `--delay` | Índice do item para cálculo do delay (número puro, sem `s`) | `1`, `2`, `3`... |

---

## ✨ Funcionalidades

- **Animação infinita** — loop contínuo sem saltos visíveis
- **Direção reversa** — classe `.reverse` inverte o sentido do movimento
- **Pausa no hover** — ao passar o mouse sobre o container, todos os itens pausam
- **Destaque no hover** — o item sob o cursor mantém a cor original enquanto os demais ficam em escala de cinza
- **Máscara de fade** — bordas esquerda e direita com fade transparente para suavizar a entrada e saída dos itens
- **Responsivo** — tamanhos e velocidades adaptados para mobile, tablet e desktop

---

### Adicionar mais itens

1. Adicione a imagem em `images/`
2. Adicione um novo `.item` no HTML seguindo a sequência do `--delay`
3. Atualize o `--quantity` no container para refletir o novo total

---

## 🛠️ Tecnologias

- HTML5
- CSS3 (animações, variáveis customizadas, media queries, `mask-image`)

---

## 📄 Licença

Este projeto é de uso livre para fins educacionais e pessoais.