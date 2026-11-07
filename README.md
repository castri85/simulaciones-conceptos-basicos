# Laboratorio de física

Una aplicación independiente para explorar ondas, sonido, movimiento rectilíneo uniforme y vectores. Incluye recorridos breves, controles, simulaciones, gráficas, tablas y preguntas opcionales. No requiere cuentas, servidor, instalación ni conexión para funcionar.

## Abrir y utilizar

Abre `Fisica-interactiva.html` mediante doble clic. `index.html` contiene exactamente la misma aplicación para su publicación web. Elige un módulo, reproduce o mueve la barra de tiempo y cambia las magnitudes. Desliza las barras para cambiar los valores; el número aparece junto a cada magnitud. «Comparar» guarda el estado actual como referencia hasta pulsarlo de nuevo; «Restablecer» recupera los valores iniciales. En móviles se puede deslizar horizontalmente dentro de las escenas y gráficas.

Las opciones CSV y PNG descargan la tabla de datos o una imagen de la gráfica. CSV incluye parámetros y unidades; el separador de columnas es la coma y los decimales se guardan con punto. Los botones de apariencia permiten cambiar a tema claro o alto contraste. No se reproducen sonidos ni se recogen datos personales.

## Modelos y alcance

- **Ondas:** onda sinusoidal viajera, `y = A sen(2πx/λ − 2πft)`, o superposición estacionaria `y = 2A sen(2πx/λ) cos(2πft)`. El extremo de la cuerda estacionaria está en `L = nλ/2`; `v = λf` describe las ondas componentes. Las escalas visuales se adaptan para mantener la escena visible.
- **Sonido:** partículas longitudinales y presión relativa; aire seco con `v ≈ 331 + 0,6θ` m/s entre 0 y 40 °C, y agua a 1500 m/s como aproximación. `h = vt/2` para el eco. El ancho representado se ajusta a dos longitudes de onda; el pulso de eco usa una distancia visual comprimida.
- **MUR:** `x = x₀ + vt`, sin aceleración. En el modo de dos móviles se calcula el encuentro con ambas posiciones. El tiempo negativo se muestra como encuentro pasado. El valor interno de velocidad es m/s y la conversión a km/h usa un factor de 3,6.
- **Vectores:** suma, resta y multiplicación por escalar a partir de componentes. Las flechas usan escalas iguales en ambos ejes; la dirección se calcula con `atan2` y no se define para el vector nulo. Las barras permiten ajustar las componentes en pasos de 0,1 unidades.

Las simulaciones son idealizaciones educativas, no un instrumento de medición. No hay audio. El modo de vectores utiliza la construcción punta-cola y no incluye una construcción de paralelogramo independiente ni puntos P y Q. La comparación de sonido muestra en la gráfica la señal anterior; no representa dos pulsos de eco simultáneos. Las escenas guiadas ofrecen texto y saltos temporales, sin una narración de audio. Las preferencias no se guardan entre visitas.

## GitHub Pages

El sitio está preparado para una rama `main` y carpeta raíz `/`. En el repositorio, abre **Settings → Pages**, selecciona **Deploy from a branch**, elige `main` y `/(root)`, y guarda. Espera a que finalice la publicación y usa el enlace mostrado en esa página. Las rutas son relativas y no dependen de bibliotecas externas. Consulta la [documentación oficial de GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

