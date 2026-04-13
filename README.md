# Tailwind CSS - Anotações

O Tailwind é um framework de CSS. Com ele, você utiliza classes diretamente no HTML
para fazer a estilização, sem precisar criar um arquivo CSS separado.

A estilização é feita inline (no próprio HTML).

---

## 📏 UNIDADES

O Tailwind usa principalmente REM (não pixels).

Exemplo:
<h1 class="m-4">Oi</h1>

4 → 4 * 0.25rem = 1rem = 16px

Também é possível usar valores personalizados:

<h1 class="m-[16px]">Oi</h1>

---

## 🧩 PADRÃO DAS CLASSES

Geralmente segue o padrão:

propriedade-valor

Ex:
text-lg
bg-blue-500
p-4

---

## 📦 ESPAÇAMENTOS

margin -> m
margin-bottom -> mb
margin-top -> mt
margin-left -> ml
margin-right -> mr
margin eixo x (left + right) -> mx
margin eixo y (top + bottom) -> my

padding -> p
padding-right -> pr
padding-left -> pl
padding-top -> pt
padding-bottom -> pb

---

## 🎨 CORES

background-color -> bg
color (texto) -> text

Exemplo com escala do Tailwind:
<h1 class="bg-blue-500">Oi</h1>

⚠️ (corrigido: você escreveu bg-blue-5005, o certo é 500)

Também pode usar valor customizado:
<h1 class="bg-[#ff00ff]">Oi</h1>

---

## 🔤 FONTES

Tamanho do texto:
text-sm
text-lg
text-xl
text-2xl

Ex:
<h1 class="text-white text-2xl">Oi</h1>

Peso da fonte:

<h1 class="font-bold">Oi</h1>
(font-weight: 700)

---

## 🔠 ESPAÇAMENTO ENTRE LETRAS

<h1 class="tracking-widest">Oi</h1>

---

## 📐 DISPLAY (FLEXBOX & GRID)

Flex:

display: flex;

<h1 class="flex">Oi</h1>

Direção:

<h1 class="flex flex-col">Oi</h1>

(row é padrão)

---

Grid:

grid-template-columns: repeat(3, minmax(0, 1fr));

<h1 class="grid grid-cols-3">Oi</h1>

---

## 📏 TAMANHO

height -> h
width -> w

Ex:
<button class="h-12 w-24">Click me</button>

Altura total da tela:
h-screen

Altura total do elemento pai:
h-full

---

## 📉 TAMANHOS MÍNIMOS

min-width -> min-w
min-height -> min-h

Ex:
<div class="min-h-screen"></div>

---

## 🎯 ESTADOS (HOVER, ETC)

Formato:
estado:propriedade-valor

Ex:
<button class="hover:bg-red-500 hover:text-white">
  Click me
</button>

---

## 📱 BREAKPOINTS (RESPONSIVIDADE)

São pontos onde o layout muda dependendo do tamanho da tela.

Exemplo equivalente ao @media no Tailwind:

sm -> 640px
md -> 768px
lg -> 1024px
xl -> 1280px

Ex:
<div class="bg-red-500 md:bg-blue-500 lg:bg-green-500"></div>

Resultado:
mobile -> sm
tablet -> md
desktop -> lg

---

## CONCLUSÃO

Estudo feito por meio do video da Fernanda Kipper - CURSO DE TAILWIND PARA INICIANES | Tutorial Tailwind do ZERO e documentação Tailwind
Link: https://www.youtube.com/watch?v=DL3IPyEXRKU

Documentação do Tailwind
https://tailwindcss.com/docs/