# Calculadora y conversor · Grupo 4 · ET403 (Semana 9)

Calculadora de suma, resta, multiplicación y división (versión de la semana 7), mejorada con un **conversor de unidades**: metros ↔ centímetros y kilogramos ↔ gramos.

## Enlaces
- Repositorio: https://github.com/juanhuaycamacarihuasairo-arch/calculadora-grupo4
- Sitio publicado (GitHub Pages): https://github.com/juanhuaycamacarihuasairo-arch

## Archivos
| Archivo | Función |
|---|---|
| `index.html` | Estructura: calculadora y sección del conversor |
| `styles.css` | Estilos base + personalización (paleta azul RGB(30, 64, 175), título de 2rem) |
| `app.js` | Lógica: calculadora original y conversor (lista `conversiones` + función `convertir`) |
| `index-original.html` | Copia de la calculadora original de la semana 7 |

## Uso
1. **Calculadora:** escriba dos datos, elija la operación y pulse *Calcular*.
2. **Conversor:** escriba un valor (0 o mayor), elija la conversión y pulse *Convertir*.
3. Se rechazan: campo vacío, texto o número no finito y valores negativos (en el conversor). La calculadora rechaza vacío, texto y división entre cero.

## Personalización
- Etiqueta HTML cambiada: `<h1>` → «Calculadora y conversor · Grupo 4», tamaño `2rem` (antes `1.5rem`).
- Paleta: azul RGB(30, 64, 175); texto blanco sobre ese azul con contraste ≈ 8,7 : 1.

## Aportes del grupo
Integrante	Tema que debe dominar	Pregunta de sustentación y respuesta clave
RODAS GUERRERO, JUAN CARLOS (líder)	Organización del proyecto en archivos	¿Por qué se separó el código en index.html, styles.css y app.js? Cada archivo tiene una función: estructura, estilos y comportamiento. Se enlazan con link y script, y se conservó index-original.html como copia de la semana 7.
CHICOMA CRUZADO, ANTONELLA ALEXANDRA	Lista de objetos y función convertir ()	¿Qué diferencia hay entre la lista conversiones y la función convertir ()? La lista guarda los datos (origen, destino, factor, operación) y la función ejecuta el cálculo. Para agregar una conversión basta añadir un objeto.
HUAICAMA CARIHUASAIRO, JUAN ROBERTO	Validaciones del conversor	¿Qué devuelve Number("abc") y cómo se detecta? Devuelve NaN; Number.isFinite() da false y se muestra escriba un número válido. Además, se rechazan el campo vacío y los valores negativos.
REATEGUI PANDO, MIREYA CLEMENTINA	Fórmulas y factor de conversión	¿Cómo se convierte 1? 5 m a cm y 1000 g a kg? Con operación multiplicar, 1.5 × 100 = 150 cm; con dividir, 1000 ÷ 1000 = 1 kg.
REQUEJO VILAS, MARY CIELO	Selector, eventos e identificadores propios	¿Cómo se llena el select y por qué los identificadores son distintos de los de la calculadora? Se recorre la lista con forEach y se crean option; los ids propios (valorConv, tipoConv…) evitan conflictos con a, b, operacion, calcular y resultado.
YAMPIS TARIMO, DATSA PAULO	Pruebas: casos normales, límite e inválidos	¿Cuál es un caso normal, uno límite y uno inválido de su tabla? Normal: 1 m a cm. Límite: 0 m a cm. Inválido: vacío, abc o -5. Compara lo esperado con lo obtenido en cada uno.
BAKUANTS UWAK, YUNI LEZZY	Personalización y publicación	¿Qué se personalizó y por qué es accesible? Título en 2rem (antes 1.5rem) y paleta azul RGB (30, 64, 175); el contraste con texto blanco es de 8,7: 1, sobre el mínimo de 4,5: 1. Luego se publica en GitHub Pages.

