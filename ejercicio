/*
Este código define la función calcularMontoAlquiler, que toma tres parámetros: 
tipoVehiculo (cadena de texto que representa el tipo de vehículo), 
diasAlquiler (número de días de alquiler) y sillaBebe (booleano que indica
si se requiere una silla para bebé).
Dentro de la función, se utiliza una declaración switch para determinar 
el costo por día según el tipo de vehículo proporcionado. Luego, se realiza 
el cálculo del costo total multiplicando el costo por día por el número de días de alquiler.
Si sillaBebe es true, se agrega un costo adicional por día para la silla 
para bebé, y se actualiza el costo total.
Finalmente, se construye un mensaje que muestra el tipo de vehículo, los días 
utilizados y el costo total. Si se requirió la silla para bebé, se incluye esa 
información en el mensaje.
En el ejemplo de uso proporcionado, se llama a la función calcularMontoAlquiler 
con los valores 'compacto' para tipoVehiculo, 3 para diasAlquiler y true para 
sillaBebe. El resultado se muestra en la consola.
*/

function calcularMontoAlquiler(tipoVehiculo, diasAlquiler, sillaBebe) {
  var costoPorDia;

  switch (tipoVehiculo) {
    case 'compacto':
      costoPorDia = 14000;
      break;
    case 'mediano':
      costoPorDia = 17000;
      break;
    case 'camioneta':
      costoPorDia = 28000;
      break;
    default:
      console.log('Tipo de vehículo no válido');
      return;
  }

  var costoTotal = costoPorDia * diasAlquiler;

  if (sillaBebe) {
    var costoSillaBebe = 1200 * diasAlquiler;
    costoTotal += costoSillaBebe;
  }

  var mensaje = 'Estimado cliente: en base al tipo de vehículo ' + tipoVehiculo + ' alquilado, considerando los ' + diasAlquiler + ' días utilizados';

  if (sillaBebe) {
    mensaje += ', con silla para bebé';
  }

  mensaje += ', el monto total a pagar es de $' + costoTotal + '.';

  console.log(mensaje);
}

// Ejemplo de uso
calcularMontoAlquiler('compacto', 3, true);
