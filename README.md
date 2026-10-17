# Pizarra del Coach

App web para que entrenadores planifiquen la semana de entrenamiento de sus alumnos.

## Funciones

- **Hoy:** qué alumnos entrenan hoy y con qué ejercicios.
- **Alumnos:** ficha con objetivo, nivel y notas, y plan semanal de lunes a domingo (series, repeticiones, carga, descanso y notas).
- **Volumen:** tonelaje por ejercicio, día y semana, series semanales por músculo (18 grupos) y evolución semana a semana.
- **Progreso:** registro de peso corporal, cintura, % de grasa o carga por ejercicio, con gráfico.
- **Ejercicios:** biblioteca propia con músculo principal y secundarios, y una base de 26 ejercicios para empezar.

## Dónde quedan los datos

Todo se guarda en el navegador de cada persona (localStorage). No hay servidor ni cuentas: cada entrenador que abre la app tiene sus propios datos, y nadie más puede verlos.

Por eso conviene usar **Alumnos → Respaldo de datos → Exportar respaldo** de vez en cuando. El archivo `.json` sirve para:

- recuperar los datos si se borra el navegador;
- pasar los datos a otro teléfono o computador con **Importar respaldo**.

Los datos no se sincronizan solos entre dispositivos.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `pizarra-coach`). Puede ser público.
2. Sube el archivo `index.html` (y este `README.md`) a la raíz del repositorio con **Add file → Upload files**.
3. Ve a **Settings → Pages**.
4. En **Build and deployment**, elige **Deploy from a branch**, la rama `main` y la carpeta `/ (root)`. Guarda.
5. En uno o dos minutos la app queda en `https://<tu-usuario>.github.io/pizarra-coach/`.

Comparte ese enlace con otros entrenadores. En el teléfono pueden usar **Agregar a pantalla de inicio** para abrirla como app.

## Desarrollo

Es un solo archivo HTML sin dependencias ni paso de compilación. Usa fuentes de Google Fonts; sin conexión cae a fuentes del sistema.
