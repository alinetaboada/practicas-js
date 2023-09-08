# practicas-js
// Generar un número aleatorio para la posición inicial entre 0 y 359 grados
const posicionInicial = Math.floor(Math.random() * 360);

// Generar un número aleatorio para la cantidad de vueltas entre 5 y 10
const vueltas = Math.floor(Math.random() * 6) + 5;

// Calcular el ángulo final
const anguloFinal = (posicionInicial + vueltas * 360) % 360;

// Imprimir los resultados
console.log(`Posición o ángulo Inicial G.A.: ${posicionInicial}`);
console.log(`Valor Aleatorio Generado en Grados: ${vueltas * 360}`);
console.log(`Ángulo Final: ${anguloFinal}`);
