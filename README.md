### Ejercicio WEATHER INFO 

Vamos a practicar **useEffect** y asincronía con React

- Un **Componente WeatherList** que recorra una lista de items con la información del pronóstico extendido de los próximos días. 
- Un **Componente WeatherCard** que contenga la información meteorológica de las próximas horas ese día (horario, temperatura, estado del tiempo (ej: clear, clouds, rain))
- Un formulario con input + botón para buscar una ciudad en concreto.

### Flujo de esta vista: 
- En esta vista se mostrará por defecto el pronóstico extendido de Madrid. Al introducir una nueva ciudad en el input de tipo texto y hacer click en el botón, la información se actualizará con los datos correspondientes a la ciudad buscada. 
- *EXTRA 1:* Agregar al componente una imágen que ilustre el estado del tiempo de cada día.
- *EXTRA 2:* En la primera carga de datos de esta vista, reemplazar Madrid por la geolocalización actual del usuario. 

TIP: usad el paquete de NPM UUID para manejar las keys de los diferentes elementos de la lista.
- [UUID](https://www.npmjs.com/package/uuid)
- [Sobre formularios](https://es.reactjs.org/docs/forms.html)
- [API Weather | 3-hour Forecast 5 days](https://openweathermap.org/forecast5)

### Para utilizar .env en proyecto con React + Vite

- .env
```js
VITE_SOME_KEY=123
DB_PASSWORD=foobar
```
- Código JS a añadir en tu componente para usar variables de entorno
```js
console.log(import.meta.env.VITE_SOME_KEY) // "123"
console.log(import.meta.env.DB_PASSWORD) // undefined
```

- Tutoriales
  - [.env react + vite](https://vite.dev/guide/env-and-mode)
  - [how-to-use-environment-variables-in-vite-react](https://dev.to/orama254/how-to-use-environment-variables-in-vite-react-template-example-34ff)