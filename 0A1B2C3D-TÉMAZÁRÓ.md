## Témazáró | Bevezetés a JavaScriptbe
#### Number - Variables



#### Számok összege

Adj össze három egész számot: 3, 15 és 20. Írasd ki az eredményt a konzolra.

```js
let összeadás = 3 [1] 15 [2] 20;
[3]
```

---

#### Kör kerülete

Egy kör sugara 15 egység. Számítsd ki a kör kerületét az alábbi képlettel:



```js
let radius = [4]; 
let circumference = 2 * [5] * [6]; 

[7](`A kör kerülete: [8].[9] egység`);
```


---

## Adó kiszámítás

Egy termék ára 19,99 Ft, az ÁFA 27%. Számítsd ki és írasd ki:

Az ÁFA összegét.
A termék végső árát ÁFA-val együtt.


```js
let price = 19.99; 
let taxRate = 0.27; 

let taxAmount = [10] * [11]; 
let finalPrice = [12] + [13]; 

console.log([14]);
console.log([15]);
```

---

## Kamatos kamat kiszámítása

Egy banki befektetés 100,000 Ft, az éves kamatláb 5%, és a pénz 3 évig kamatozik. Számítsd ki, hogy mennyi lesz a befektetés értéke a 3 év után.


```js
let principal = 100000; 
let interestRate = 0.05; 
let years = 3; // Évek száma

let totalAmount = principal * [16]; 

console.log([17]);
```

---

## Fény utazási ideje


A Hold távolsága a Földtől körülbelül 384,400 km, a fény sebessége 299,792 km/s.

Számítsd ki, mennyi idő alatt ér el a fény a Holdról a Földre másodpercben.

```js
let moonDistance = 384400; 
let lightSpeed = 299792; 

let travelTime = [18] / [19]; 

console.log([20]);
```

---

## Legkisebb érték kiválasztása

Válaszd ki a legkisebb értéket a következő számok közül: 34, 8, 19.

```js
const result7 = [21];
console.log([22]);
```
---

## Template Literals

Van két változód: a = "Alice" és b = 25. Írj ki egy mondatot a konzolra a következő formátumban:

```js
const a = "Alice";
const b = 25;
console.log([23]);
```

---

## Összehasonlítás

észíts egy JavaScript kódot, ami két számot hasonlít össze, és kiírja, hogy az első szám nagyobb-e a másodiknál. Ha igaz, akkor a "Az első szám nagyobb" üzenet jelenjen meg, különben a "Az első szám nem nagyobb" üzenet

```js
let a = 10;
let b = 5;
[25] ([26]) {
console.log("Az első szám nagyobb");
} [27] {
console.log("Az első szám nem nagyobb");
    }
```

---

## Páros vagy páratlan

Írj egy kódot, amely ellenőrzi, hogy egy adott szám páratlan vagy páros. A kimenet "Páros" vagy "Páratlan" legyen, a szám alapján.


```js
let szam = 7;
[28] ([29]) {
    console.log("Páros");
} [30] {
    console.log("Páratlan");
}
```

---

## Egyenlő vagy sem

```js
let nev1 = "Anna";
let nev2 = "Anna";
[31] ([32]) {
    console.log("A két név egyenlő");
} [33] {
    console.log("A két név nem egyenlő");
}
```

---
 ## null or undefined

 mi lesz a várható eredmény és miért?

 [34](null == undefined)

 [35](null === undefined)

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

[36] ([37]) {
    console.log("Az e-mail cím nincs beállítva.");
} [38] {
    console.log("Felhasználó e-mail címe:", userProfile.email);
}
```
---

## Globális változó

ezek közül melyik egy globális és melyik egy blokk szintű változó:



[39]
```js
var változó1 = "Hello, world!";
console.log(window.változó1); // "Hello, world!"
```

[40]
```js
function myFunction() {
  var változó2 = { name: "John", age: 30 };
  console.log(változó2.name);  // "John"
}

myFunction();
console.log(változó2);  // Error: localObj is not defined
```

---

## final boss

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
    [41]Idézet Generátor[41]
    <div [42]="idezetDoboz" [43]="idezet">Választott idézet: ?</div>

    <script>
        [44] idezetek = [
            { szoveg: "A siker nem végleges, a kudarc nem végzetes: a bátorság számít, hogy folytasd.", szerzo: "Winston Churchill" },
            { szoveg: "Az egyetlen módja annak, hogy nagyszerű munkát végezz, ha szereted, amit csinálsz.", szerzo: "Steve Jobs" },
            { szoveg: "Ne számold a napokat, tedd a napokat számításba.", szerzo: "Muhammad Ali" },
            { szoveg: "Az élet 10%-ban az, ami veled történik, és 90%-ban az, ahogyan reagálsz rá.", szerzo: "Charles R. Swindoll" }
        ];

        let valasztottSzam = [45]("Válassz egy számot 1 és 4 között:");
        valasztottSzam = [46](valasztottSzam);

        [47]
        let kivalasztottIdezet;

        if ([48]) {
            [49];
        } else if ([50]) {
            [51];
        } else if ([52]) {
            [53];
        } else {
            [54];
        }

        [55].[getElementById]([56]).innerText = `"[57]" - [58]`;
    </script>
</body>
</html>
```
