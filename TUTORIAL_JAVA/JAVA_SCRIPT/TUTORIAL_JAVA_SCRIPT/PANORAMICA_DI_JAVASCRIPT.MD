## Panoramica del linguaggio JavaScript

Si trova qui:

	https://developer.mozilla.org/en-US/docs/Web/JavaScript/Language_Overview#objects

JavaScript è un linguaggio dinamico multiparadigma con tipi e operatori, oggetti predefiniti standard e metodi. La sua sintassi è basata sui linguaggi Java e C - molte strutture di quei linguaggi si applicano anche a JavaScript. JavaScript supporta la programmazione orientata agli oggetti con prototipi di oggetti e classi. Supporta anche la programmazione funzionale poiché le funzioni sono di prima classe che possono essere facilmente create tramite espressioni e passate come qualsiasi altro oggetto.
Questa pagina serve come una rapida panoramica delle varie funzionalità del linguaggio JavaScript, scritte per i lettori con esperienza in altri linguaggi, come C o Java.

## Tipi di dati
Iniziamo osservando gli elementi costitutivi di qualsiasi linguaggio: i tipi. I programmi JavaScript manipolano i valori e questi valori appartengono tutti a un tipo. JavaScript offre sette tipi primitivi:

1) Numero: utilizzato per tutti i valori numerici (intero e virgola mobile) ad eccezione dei 
			numeri interi molto grandi.
2) BigInt: utilizzato per numeri interi arbitrariamente grandi.
3) String: utilizzato per memorizzare il testo.
4) Boolean: e — solitamente usato per la logica condizionale.truefalse
5) Symbol: utilizzato per creare identificatori univoci che non si scontrano.
6) Undefined: indica che a una variabile non è stato assegnato un valore.
7) Null: indica un non-valore deliberato.

Tutto il resto è conosciuto come un oggetto. I tipi di oggetto comuni includono:

- Function: Le funzioni non sono strutture di dati speciali in JavaScript: sono solo un tipo speciale di oggetto che può essere chiamato.
- Array
- Date
- RegExp
- Error

JavaScript ha due tipi numerici incorporati: Number e BigInt.
###	Numeri

Il tipo Number è un valore in virgola mobile a doppia precisione IEEE 754 a 64 bit, il che significa che i numeri interi possono essere rappresentati in modo sicuro tra -(2 53 − 1) e 253 − 1 senza perdita di precisione, e i numeri in virgola mobile possono essere memorizzati fino a 1.79 × 10308. All'interno dei numeri, JavaScript non distingue tra numeri a virgola mobile e numeri interi.

	console.log(3 / 2); // 1.5, not 1


			