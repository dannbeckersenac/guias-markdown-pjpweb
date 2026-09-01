# regras.md: tela de [NOME DA PERSONA] em React

Este arquivo vai junto com todo prompt que eu mandar para a IA nesta atividade.
Ele diz quem usa a tela, o que ela precisa ter, o que eu ja sei e o que eu ainda
nao aprendi. Sem ele, a IA entrega uma tela generica para um usuario que nao existe.

---

## 1. Quem usa esta tela

[Copiar da folha de persona: nome, idade, trabalho, situacao de uso.
Tres a quatro linhas. Incluir o que atrapalha o uso: mao, olho, luz,
interrupcao, memoria, tempo.]

Frase da persona:

> "[Copiar a frase exata da carta.]"

---

## 2. O que a tela e obrigada a ter

Cada item abaixo veio de uma parte da frase ou do perfil. A IA nao pode ignorar
nenhum deles. Se ignorar, eu recuso o codigo.

| A persona diz ou vive | A tela e obrigada a ter |
|---|---|
| [trecho da persona] | [requisito concreto: tamanho, cor, posicao, quantidade de toques] |
| [trecho da persona] | [requisito concreto] |
| [trecho da persona] | [requisito concreto] |
| [trecho da persona] | [requisito concreto] |
| [trecho da persona] | [requisito concreto] |

---

## 3. O que a tela nao pode ter

- [Exemplo: campo para digitar valor]
- [Exemplo: icone sem texto]
- [Exemplo: elemento que some depois de usado]
- [Preencher com o que a persona proibe, mesmo sem dizer com essas palavras]

---

## 4. O que eu ja sei e o codigo deve usar

- Projeto criado com Vite (`npm create vite@latest`, template react)
- Componentes escritos com `function`, um por arquivo, na pasta `src/componentes`
- JSX: `className`, chaves `{}` para valor, uma raiz por `return`
- Props recebidas com desestruturacao: `function Botao({ nome, aoTocar })`
- `useState` no componente mais alto que precisa do dado (em geral o `App`)
- Lista na tela com `map` e `key` vinda do id do item, nunca da posicao
- Eventos com `onClick`, chamando funcao recebida por props
- Dados fixos da tela (lista de itens, precos) em um arquivo na pasta `src/dados`
- O CSS da minha versao anterior, reaproveitado sem mudanca

---

## 5. O que eu ainda nao aprendi e o codigo nao pode ter

- `useEffect`, `useContext`, `useReducer` ou qualquer outro hook alem de `useState`
- Bibliotecas de componentes (Material UI, Chakra, Bootstrap React) ou de estilo (styled-components, Tailwind)
- Rotas, estado global, `localStorage`, `fetch`
- `innerHTML`, `var`, `==`
- `document.querySelector` dentro de componente
- `push` em lista que esta no estado
- Funcao com seta fora de `onClick` e de `map`
- TypeScript, testes automatizados, animacao

Se a IA achar que precisa de algo desta lista, ela deve parar e me explicar por que,
em vez de usar.

---

## 6. Como eu quero que o codigo chegue

- Nomes de componentes, funcoes, variaveis e props em portugues, sem acento
- Comentarios dizem POR QUE a linha existe, ligando ao requisito da persona.
  Comentario que so repete o que a linha faz sera apagado
- Toda decisao de tela que afeta a persona (tamanho, cor, ordem, o que aparece)
  vem marcada com `// DECISAO SUA:` e uma frase explicando a escolha
- Deixar exatamente tres lacunas marcadas com `// COMPLETAR:` que eu vou escrever
  a mao: [escolher: a funcao que altera o estado / o map / o componente do total]
- Antes de eu rodar, eu escrevo o que espero ver. A IA nao roda por mim

---

## 7. Ponto de partida

O codigo abaixo e a minha tela atual, em HTML, CSS e JavaScript puros. A tarefa
e MIGRAR esta tela para React, nao inventar outra. A aparencia final tem que ser a mesma.

### index.html

```html
[colar]
```

### script.js

```js
[colar]
```

### estilo.css

Nao precisa reescrever. Sera copiado para `src/estilo.css` sem alteracao.
