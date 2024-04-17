1 - Trova tutte le risorse con il dato isActive corrispondente a true

{isActive: {$eq:true}}
51 risorse trovate


2 - Trova tutte le risorse con il dato age maggiore di 26

{age: {$gt:26}}
54 risorse trovate


3 - Trova tutte le risorse con il dato age maggiore di 26 e minore o uguale a 30

{$and:[{age: {$gt:26}}, {age:{$lte:30}}]}
19 risorse trovate


4 - Trova tutte le risorse con il dato eyes che sia brown o blue

{$or:[{"eyeColor": "brown"}, {"eyeColor":"blue"}]}
66 risorse trovate


5 - Trova tutte le risorse che non presentano il dato eyes uguale a green

{"eyeColor":{$not:/^green.*/}}
66 risorse trovate


6 - Trova tutte le risorse che non presentano il dato eyes uguale a green e neanche blue

{$nor:[{"eyeColor":"green"}, {"eyeColor":"blue"}]}
35 risorse trovate


7 - Trova tutte le risorse con il dato company uguale a "FITCORE" e ritorna solo l'email

{"company": "FITCORE"}
project: {"email": 1}
1 risorsa trovata