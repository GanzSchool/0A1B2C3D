## Témazáró | Bevezetés a JavaScriptbe
#### Number - Variables



#### Számok összege

Adj össze három egész számot: 3, 15 és 20. Írasd ki az eredményt a konzolra.

```js
let összeadás = 3 + 15 + 20
console.log(összeadás)
```

---

#### Kör kerülete

Egy kör sugara 15 egység. Számítsd ki a kör kerületét az alábbi képlettel:

Kerület = 2 × r × π
👉 Használj Math.PI-t a π értékére.

```js
let radius = 7; // A kör sugara
let circumference = 2 * radius * Math.PI; // Kör kerülete

console.log(`A kör kerülete: ${circumference.toFixed(2)} egység`);
```


---

## Adó kiszámítás

Egy termék ára 19,99 Ft, az ÁFA 27%. Számítsd ki és írasd ki:

Az ÁFA összegét.
A termék végső árát ÁFA-val együtt.
👉 Tipp: Használj toFixed()-et a kerekítéshez. Kerekítsd az eredményeket két tizedesjegyre.

```js
let price = 19.99; // Termék ára
let taxRate = 0.27; // ÁFA-kulcs (27%)

let taxAmount = price * taxRate; // ÁFA összege
let finalPrice = price + taxAmount; // Végső ár ÁFA-val együtt

console.log(`ÁFA összege: ${taxAmount.toFixed(2)} Ft`);
console.log(`Végső ár: ${finalPrice.toFixed(2)} Ft`);
```

---

## Kamatos kamat kiszámítása

Egy banki befektetés 100,000 Ft, az éves kamatláb 5%, és a pénz 3 évig kamatozik. Számítsd ki, hogy mennyi lesz a befektetés értéke a 3 év után.

👉 Képlet: Végösszeg = befektetés × (1 + kamatláb)^évek. Használd a Math.pow() metódust a hatványozás kiszámítására.

```js
let principal = 100000; // Befektetés összege
let interestRate = 0.05; // Éves kamatláb (5%)
let years = 3; // Évek száma

let totalAmount = principal * Math.pow(1 + interestRate, years); // Kamatos kamat képlet

console.log(`A befektetés értéke 3 év után: ${totalAmount.toFixed(2)} Ft`);
```

---

## Fény utazási ideje


A Hold távolsága a Földtől körülbelül 384,400 km, a fény sebessége 299,792 km/s.

Számítsd ki, mennyi idő alatt ér el a fény a Holdról a Földre másodpercben.

```js
let moonDistance = 384400; // Hold távolsága km-ben
let lightSpeed = 299792; // Fény sebessége km/s-ban

let travelTime = moonDistance / lightSpeed; // Idő = távolság / sebesség

console.log(`A fény utazási ideje a Holdtól a Földig: ${travelTime.toFixed(2)} másodperc`);
```

---

## Legkisebb érték kiválasztása

Válaszd ki a legkisebb értéket a következő számok közül: 34, 8, 19.

```js
const result7 = Math.min(34, 8, 19);
console.log(`A legkisebb szám: ${result7}`);
```
---

## Template Literals

Van két változód: name = "Alice" és age = 25. Írj ki egy mondatot a konzolra a következő formátumban:
"Alice 25 éves." (Használj template literált.)

```js
const name = "Alice";
const age = 25;
console.log(`${name} ${age} éves.`);
```

---

## Falsy Truea

Ezek közül add meg melyik treethy és melyik falshy

---


## Összehasonlítás

észíts egy JavaScript kódot, ami két számot hasonlít össze, és kiírja, hogy az első szám nagyobb-e a másodiknál. Ha igaz, akkor a "Az első szám nagyobb" üzenet jelenjen meg, különben a "Az első szám nem nagyobb" üzenet

```js
let a = 10;
let b = 5;
if (a > b) {
console.log("Az első szám nagyobb");
} else {
console.log("Az első szám nem nagyobb");
    }
```

---

## Páros vagy páratlan

Írj egy kódot, amely ellenőrzi, hogy egy adott szám páratlan vagy páros. A kimenet "Páros" vagy "Páratlan" legyen, a szám alapján.


```js
let szam = 7;
if (szam % 2 === 0) {
    console.log("Páros");
} else {
    console.log("Páratlan");
}
```

---

## Egyenlő vagy sem

```js
let nev1 = "Anna";
let nev2 = "Anna";
if (nev1 === nev2) {
    console.log("A két név egyenlő");
} else {
    console.log("A két név nem egyenlő");
}
```

---
 ## null or undefined

 mi lesz a várható eredmény és miért?

 (null == undefined)

 (null === undefined)

---


## Profil beállításai – Hiányzó tulajdonságok kezelése

Hozz létre egy userProfile nevű objektumot, amely egy name tulajdonságot tartalmaz.
Ellenőrizd, hogy van-e email tulajdonsága az objektumnak.
Ha nincs email tulajdonság (azaz az undefined), írj ki egy üzenetet: "Az e-mail cím nincs beállítva."
Ha van email, írd ki: "Felhasználó e-mail címe: X" (ahol X az e-mail címe).

```js
let userProfile = {
    name: "Zoltán"
};

if (userProfile.email === undefined) {
    console.log("Az e-mail cím nincs beállítva.");
} else {
    console.log("Felhasználó e-mail címe:", userProfile.email);
}
```
---

## Globális változó

ezek közül melyik egy globális és melyik egy blokk szintű változó:


Mi az a globális változó?

```js
var myGlobalVar = "Hello, world!";
console.log(window.myGlobalVar); // "Hello, world!"
```

```js
function myFunction() {
  var localObj = { name: "John", age: 30 };
  console.log(localObj.name);  // "John"
}

myFunction();
console.log(localObj);  // Error: localObj is not defined
```

---

## nagy feladat

```html
<!DOCTYPE html>
<html lang="hu">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Idézet Generátor</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            background: linear-gradient(135deg, #8e44ad, #3498db);
            color: #fff;
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
        }
        .idezet {
            font-size: 24px;
            font-weight: bold;
            padding: 20px;
            border: 3px solid white;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 10px;
            margin-top: 20px;
            max-width: 600px;
        }
    </style>
</head>
<body>
    <h1>Idézet Generátor</h1>
    <div id="idezetDoboz" class="idezet">Választott idézet: ?</div>

    <script>
        const idezetek = [
            { szoveg: "A siker nem végleges, a kudarc nem végzetes: a bátorság számít, hogy folytasd.", szerzo: "Winston Churchill" },
            { szoveg: "Az egyetlen módja annak, hogy nagyszerű munkát végezz, ha szereted, amit csinálsz.", szerzo: "Steve Jobs" },
            { szoveg: "Ne számold a napokat, tedd a napokat számításba.", szerzo: "Muhammad Ali" },
            { szoveg: "Az élet 10%-ban az, ami veled történik, és 90%-ban az, ahogyan reagálsz rá.", szerzo: "Charles R. Swindoll" }
        ];

        let valasztottSzam = prompt("Válassz egy számot 1 és 4 között:");
        valasztottSzam = parseInt(valasztottSzam);

        const [idezet1, idezet2, idezet3, idezet4] = idezetek;
        let kivalasztottIdezet;

        if (valasztottSzam === 1) {
            kivalasztottIdezet = idezet1;
        } else if (valasztottSzam === 2) {
            kivalasztottIdezet = idezet2;
        } else if (valasztottSzam === 3) {
            kivalasztottIdezet = idezet3;
        } else {
            kivalasztottIdezet = idezet4;
        }

        document.getElementById("idezetDoboz").innerText = `"${kivalasztottIdezet.szoveg}" - ${kivalasztottIdezet.szerzo}`;
    </script>
</body>
</html>
```