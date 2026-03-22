# Funciones Esenciales de JavaScript

## Array Methods (las más importantes)

| Función | Qué hace | Ejemplo |
|---------|----------|---------|
| `map()` | Transforma cada elemento | `[1,2,3].map(x => x*2)` → `[2,4,6]` |
| `filter()` | Filtra elementos por condición | `[1,2,3].filter(x => x>1)` → `[2,3]` |
| `reduce()` | Reduce array a un solo valor | `[1,2,3].reduce((a,b)=>a+b)` → `6` |
| `find()` | Busca primer elemento que coincide | `arr.find(x => x.id===1)` |
| `findIndex()` | Índice del primer elemento que coincide | `arr.findIndex(x => x.id===1)` |
| `some()` | ¿Alguno cumple la condición? | `[1,2,3].some(x => x>2)` → `true` |
| `every()` | ¿Todos cumplen la condición? | `[1,2,3].every(x => x>0)` → `true` |
| `forEach()` | Itera sin retornar nada | `[1,2,3].forEach(x => console.log(x))` |
| `slice()` | Copia parte del array | `[1,2,3,4].slice(1,3)` → `[2,3]` |
| `splice()` | Modifica array (añade/elimina) | `arr.splice(1,1)` → elimina 1 elemento |

## Object

| Función | Qué hace | Ejemplo |
|---------|----------|---------|
| `Object.keys()` | Array de claves | `Object.keys({a:1})` → `['a']` |
| `Object.values()` | Array de valores | `Object.values({a:1})` → `[1]` |
| `Object.entries()` | Array de `[clave, valor]` | `Object.entries({a:1})` → `[['a',1]]` |
| `Object.hasOwnProperty()` | ¿Tiene propiedad? | `obj.hasOwnProperty('a')` |

## String

| Función | Qué hace | Ejemplo |
|---------|----------|---------|
| `split()` | String → array | `"a,b,c".split(',')` → `['a','b','c']` |
| `join()` | Array → string | `['a','b'].join('-')` → `'a-b'` |
| `slice()` | Extrae parte del string | `"hello".slice(0,2)` → `'he'` |
| `replace()` / `replaceAll()` | Reemplaza texto | `"a b".replace("a","c")` → `"c b"` |
| `trim()` | Quita espacios extremos | `"  hi  ".trim()` → `'hi'` |
| `toLowerCase()` / `toUpperCase()` | Cambia caso | `"HI".toLowerCase()` → `'hi'` |
| `includes()` | ¿Contiene substring? | `"hello".includes("el")` → `true` |

## Number

| Función | Qué hace | Ejemplo |
|---------|----------|---------|
| `toFixed()` | Formato decimal | `(1.5).toFixed(2)` → `'1.50'` |
| `parseInt()` / `parseFloat()` | String → número | `parseInt("123")` → `123` |
| `isNaN()` | ¿Es NaN? | `isNaN(NaN)` → `true` |

## Otros esenciales

| Función | Qué hace | Ejemplo |
|---------|----------|---------|
| `setTimeout()` | Ejecuta después de X ms | `setTimeout(() => {}, 1000)` |
| `setInterval()` | Ejecuta cada X ms | `setInterval(() => {}, 1000)` |
| `Promise.then()` / `.catch()` | Manejo de promesas | `fetch(url).then(res => res.json())` |
| `async/await` | Promesas sintaxis limpia | `const res = await fetch(url)` |
| `JSON.stringify()` | Objeto → JSON string | `JSON.stringify({a:1})` |
| `JSON.parse()` | JSON string → objeto | `JSON.parse('{"a":1}')` |
| `console.log()` / `console.error()` | Debugging | `console.log("debug")` |

## Orden recomendado de aprendizaje

1. **map, filter, reduce** ← las 3 reinas
2. **find, some, every**
3. **Object.keys/values**
4. **String methods**
5. **Promesas (async/await)**
