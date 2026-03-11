# RA3Ex7 – Documentació del DOM amb JavaScript

Aquesta pràctica son **8 exercicis ràpids** s'utilitza selecció d'elements, modificació de contingut, atributs, estils, classes, esdeveniments, creació i eliminació de nodes.

---

## Índex d'exercicis

1. [Selecció i canvi de color](#1-selecció-i-canvi-de-color)
2. [Canvi de contingut de text](#2-canvi-de-contingut-de-text)
3. [Canvi d'atribut d'imatge](#3-canvi-datribut-dimatge)
4. [Canvi d'estil en fer clic](#4-canvi-destil-en-fer-clic)
5. [Toggle de classe CSS](#5-toggle-de-classe-css)
6. [Esdeveniment de botó amb alerta](#6-esdeveniment-de-botó-amb-alerta)
7. [Creació d'elements nous](#7-creació-delements-nous)
8. [Eliminació d'elements](#8-eliminació-delements)

---

## Exercicis i solucions

### 1. Selecció i canvi de color

> Usa `querySelector` per canviar el color d'un `<h1>` quan la pàgina carregui.

```js
let changeColor = document.querySelector("#titol-principal");
changeColor.style.color = "blue";
```


---

### 2. Canvi de contingut de text

> Fes que un paràgraf `<p>` mostri "Hola Món" usant `textContent`.

```js
let showText = document.querySelector("#paragraf-hola");
showText.textContent = "Hola Món";
```

---

### 3. Canvi d'atribut d'imatge

> Canvia la `src` d'una imatge `<img>` usant `setAttribute`.

```js
let showImg = document.getElementById("imatge-canviant");
showImg.setAttribute("src", "https://picsum.photos/150");
```


---

### 4. Canvi d'estil en fer clic

> Canvia el color de fons (`backgroundColor`) d'un element en fer-li clic.

```js
let caixaEstil = document.getElementById("caixa-estil");

caixaEstil.addEventListener("click", () => {
    caixaEstil.style.backgroundColor = "lightblue";
});
```


---

### 5. Toggle de classe CSS

> Crea un botó que afegeixi o tregui la classe `actiu` amb `classList.toggle`.

```js
let botoToggle = document.getElementById("boto-toggle");
let textClasse = document.getElementById("text-classe");

botoToggle.addEventListener("click", () => {
    textClasse.classList.toggle("actiu");
});
```


---

### 6. Esdeveniment de botó amb alerta

> Afegeix un `addEventListener` a un botó perquè mostri una alerta (`alert`).

```js
let botoAlerta = document.getElementById("boto-alerta");

botoAlerta.addEventListener("click", () => {
    alert("Hola! Has fet clic");
});
```


---

### 7. Creació d'elements nous

> Crea un nou `<li>` amb `createElement` i afegeix-lo a una `<ul>` amb `appendChild`.

```js
let botoAfegir = document.getElementById("boto-afegir");
let llista = document.getElementById("llista-compra");

botoAfegir.addEventListener("click", () => {
    let nouItem = document.createElement("li");
    nouItem.textContent = "Nou producte";
    llista.appendChild(nouItem);
});
```

---

### 8. Eliminació d'elements

> Fes que un element desaparegui en fer-li clic usant el mètode `remove()`.

```js
let elementEliminar = document.getElementById("element-eliminar");

elementEliminar.addEventListener("click", () => {
    elementEliminar.remove();
});
```

