# Nombre:
Angélica Sofía Panamá Riera

# Juego Básico del Tres en Raya
Un sencillo juego de Tres en Raya, desarrollado con HTML, CSS y JavaScript.  
Funciones: registrar jugadores, guardar partidas en el navegador y reproducir sonidos personalizados.

# Este proyecto incluye:

* Interfaz interactiva con botones e imágenes personalizadas.

* Sonidos diferentes para cada jugador y para los botones principales.

* Registro automático de partidas (ganador, duración, movimientos, fecha).

* Guardado de datos usando LocalStorage.


# Como poder ejecutarlo:

Abrir el Terminal e introducir el siguiente comando:
   python -m http.server 8000
Luego, en un navegador ingresar:
    http://localhost:8000/


# Decisiones técnicas
Su alamacenamiento utliza LocalStorage.

Se usa LocalStorage porque:

- Es fácil de implementar para datos pequeños (como partidas).

- No requiere servidor ni base de datos externa.

- Permite persistir la información incluso al cerrar el navegador.

# Cada partida se guarda como un objeto con los siguientes campos:
-Ejemplo:
{
  "jugador1": "Ana",
  "jugador2": "Luis",
  "ganador": "Ana",
  "duracion": "00:42",
  "movimientos": 6,
  "fecha": "2025-11-09 21:00:10"
}

# Lista de comprobación de estándares
- Semántica HTML: Se utilizan etiquetas adecuadas como <section>, <button>, <p>, <form> y atributos aria-live para accesibilidad.
- Accesibilidad: Colores con buen contraste, atributos aria, y lectura de turnos en texto.
- Responsividad: Diseño adaptable con CSS Grid y tamaños relativos.
- Validación HTML y CSS: Verificado con W3C Validator. No se detectaron errores críticos.
- Módulos ES6: Código dividido en game.js y storage.js para mejor mantenimiento.
- Buenas prácticas JS: Uso de funciones claras, constantes, y separación de lógica.