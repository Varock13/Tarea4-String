# **String**

## .localeCompare()

* El método localeCompare() retorna un número indicando si una cadena de carateres de referencia va antes, después o si es la misma que la cadena dada en orden alfabético.

```javascript
// La letra "a" va antes que "c" por lo que entrega un valor negativo
'a'.localeCompare('c'); // -2 o -1 (o cualquier otro valor negativo)

// Alfabéticamente la palabra "check" va después que "against" por lo que resulta
// en un valor positivo.
'check'.localeCompare('against'); // 2 o 1 (u otro valor positivo)

// "a" y "a" son equivalentes por lo que resulta en un valor neutral de cero.
'a'.localeCompare('a'); // 0
```

## .padEnd()

* El padEnd()método rellena la cadena actual con una cadena determinada (repetida, si es necesario) para que la cadena resultante alcance una longitud determinada. El relleno se aplica desde el final de la cadena actual.

```javascript
const str1 = 'Breaded Mushrooms';

console.log(str1.padEnd(25, '.'));
// expected output: "Breaded Mushrooms........"

const str2 = '200';

console.log(str2.padEnd(5));
// expected output: "200  "
```

## .padStart()

* El método padStart() rellena la cadena actual con una cadena dada (repetida eventualmente) de modo que la cadena resultante alcance una longitud dada. El relleno es aplicado desde el inicio (izquierda) de la cadena actual.

```javascript
'abc'.padStart(10);         // "       abc"
'abc'.padStart(10, "foo");  // "foofoofabc"
'abc'.padStart(6,"123465"); // "123abc"
```

## .raw()

* Se utiliza para obtener un string crudo a partir de plantillas de string (es decir, el original, texto no interpretado).

```javascript
String.raw`Hi\n${2+3}!`;
// 'Hi\n5!', El caracter despues del 'Hi'
// no es un caracter de salto de linea,
// '\' y 'n' son 2 caracteres.
```

