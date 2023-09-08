# practicas-js

// Función para simular una tirada de ruleta
function simularTirada() {
    // Genera un número aleatorio entre 5 y 10 para las vueltas de la bolilla
    const vueltas = Math.floor(Math.random() * 6) + 5;

    // Inicializa la posición en 0
    let posicion = 0;

    // Simula las vueltas de la bolilla
    for (let i = 0; i < vueltas; i++) {
        // Genera un número aleatorio entre 0 y 36 para la posición
        posicion = Math.floor(Math.random() * 37);
    }

    return { vueltas, posicion };
}

// Simula 10 tiradas e imprime los resultados
for (let juego = 1; juego <= 10; juego++) {
    const resultado = simularTirada();
    console.log(`Nro de Juego: ${juego}`);
    console.log(`Valor Aleatorio Generado: ${resultado.vueltas}`);
    console.log(`Nro que cayó en la ruleta: ${resultado.posicion}`);
    console.log();
}

