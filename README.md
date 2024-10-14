# practicaLogica
JS-05 - Práctica de lógica 
//User profile



function perfilDeUsuario() {
    const nombre = prompt("Ingresa tu nombre de usuario:");
    const edad = prompt("Ingresa tu edad:");
    const peliculasFavoritas = prompt("Ingresa tus películas favoritas separadas por comas:");

   
    const listaPeliculas = peliculasFavoritas.split(',');

  
    console.log(Nombre de usuario: ${nombre});
    console.log(Edad: ${edad});
    console.log("Películas favoritas:");
    listaPeliculas.forEach(pelicula => {
        console.log(La película ${pelicula.trim()} es una de mis favoritas.);
    });
}

perfilDeUsuario();



//Highest number


function numeroMasAlto() {
    const numeros = [];

    for (let i = 0; i < 10; i++) {
        const numero = parseFloat(prompt(Ingresa un número ${i + 1}:));
        numeros.push(numero); 
    }
    const numeroMaximo = Math.max(...numeros);
    console.log(El número más alto es: ${numeroMaximo});
}

numeroMasAlto();

//Palindrome

function esPalindromo(texto) {
  
    const texto = texto.toLowerCase().replaceAll(/[^a-z0-9]/g, '');
    const textoInvertido = texto.split('').reverse().join('');

   
    if (textoLimpio === textoInvertido) {
        console.log("Es un palíndromo");
    } else {
        console.log("No es un palíndromo");
    }
}

const palabraOFrase = prompt("Ingresa una palabra o frase:");
esPalindromo(palabraOFrase);


