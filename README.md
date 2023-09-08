# practicas-js
// Obtiene la hora actual
const horaActual = new Date();

// Obtiene la hora actual en minutos (hora * 60 + minutos)
const minutosActuales = horaActual.getHours() * 60 + horaActual.getMinutes();

// Genera un número aleatorio entre 300 (5 horas en minutos) y 600 (10 horas en minutos)
const minutosAleatorios = Math.floor(Math.random() * 301) + 300;

// Calcula la hora final en minutos sumando los minutos aleatorios a los minutos actuales
const minutosFinales = minutosActuales + minutosAleatorios;

// Convierte los minutos finales a horas y minutos
const horasFinales = Math.floor(minutosFinales / 60);
const minutosFinalesRestantes = minutosFinales % 60;

// Imprime los resultados
console.log(`Hora Actual: ${horaActual.getHours()}:${horaActual.getMinutes()}`);
console.log(`Valor Aleatorio Generado en Minutos: ${minutosAleatorios}`);
console.log(`Hora Final: ${horasFinales}:${minutosFinalesRestantes}`);
