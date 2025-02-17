## Témazáró | Bevezetés a JavaScriptbe

#### Számok összege


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

Egy termék ára 15,22 Ft, az ÁFA 22%. Számítsd ki és írasd ki az adó mértékét és a bruttó összeget!



```js
let price = 15,22;
let taxRate = 0.22;

let taxAmount = [10] * [11]; 
let finalPrice = [12] + [13];

console.log([14]);
console.log([15]);
```

---

## Kamatos kamat kiszámítása

Egy banki befektetés 100,000 Ft, az éves kamatláb 5%, és a pénz 3 évig kamatozik. Számítsd ki, hogy mennyi lesz a befektetés értéke a 3 év után.

```js
let principal = 100000; // Befektetés összege
let interestRate = 0.05; // Éves kamatláb (5%)
let years = 3; // Évek száma

let totalAmount = principal * [16]; // Kamatos kamat képlet

console.log(`A befektetés értéke 3 év után: [17] Ft`);
```

---

## Fény utazási ideje


A Hold távolsága a Földtől körülbelül 384,400 km, a fény sebessége 299,792 km/s.

Számítsd ki, mennyi idő alatt ér el a fény a Holdról a Földre másodpercben.

```js
let moonDistance = 384400;
let lightSpeed = 299792;

let travelTime = [18] / [19];

console.log(`A fény utazási ideje a Holdtól a Földig: [20] másodperc`);
```

---

## Legkisebb érték kiválasztása

Válaszd ki a legkisebb értéket a következő számok közül: 34, 8, 19.

```js
const result7 = [21](34, 8, 19);
console.log(`A legkisebb szám: [22]`);
```
---

## Template Literals

Van két változód: a = "Alice" és b = 25. Írj ki egy mondatot a konzolra a következő formátumban:
"Alice 25 éves." (Használj template literált.)

```js
const a = "Alice";
const b = 25;
console.log([23]);
```

---


## Összehasonlítás

Az alábbi kód két számot hasonlít össze, és kiírja, hogy az első szám nagyobb-e a másodiknál. Ha igaz, akkor a "Az első szám nagyobb" üzenet jelenjen meg, különben a "Az első szám nem nagyobb" üzenet.

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

Az alábbi kód ellenőrzi, hogy egy adott szám páratlan vagy páros. A kimenet "Páros" vagy "Páratlan" legyen, a szám alapján.


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


## Profil beállításai – Hiányzó tulajdonságok kezelése

Az alábbi kód egy userProfile nevű objektum szerepel, amely egy name tulajdonságot tartalmaz.
Ellenőrizd, hogy van-e email tulajdonsága az objektumnak.
Ha nincs email tulajdonság (undefined), írj ki egy üzenetet: "Az e-mail cím nincs beállítva."
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





[39]
```js
var változó1 = "Hello, world!";
console.log(window.változó1);
```

[40]
```js
function myFunction() {
  var változó2 = { name: "John", age: 30 };
  console.log(változó2.name); 
}

myFunction();
console.log(változó2);
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

        [55].[56]([57]).innerText = `"[58]" - [59]`;
    </script>
</body>
</html>
```
