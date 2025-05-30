<div> 
    <h1>Grupo 15</h1>
</div>
<div> 
    <h1>Proyecto 1</h1>
</div>
<div>
# TIMstamp (nombre del proyecto)

## 🎯 Descripción del Proyecto

_TIMstamp_ es una herramienta pensada para _creadores de contenido_ como youtubers, docentes y periodistas que trabajan con videos largos (entrevistas, clases, podcasts, etc.) y necesitan _dividir su contenido en partes_ según temas o secciones específicas.

Este proyecto permite automatizar la transcripción del video y facilita al usuario elegir _dónde cortar el video_ en bloques según la estructura del contenido.

---

## 🧠 ¿Qué problema resuelve?

Muchos creadores de contenido pierden horas revisando y cortando videos manualmente para crear partes como: Introducción, Tema 1, Tema 2, Conclusión, etc. _TIMstamp_ automatiza gran parte de ese proceso, permitiendo que el usuario simplemente elija los momentos clave y reciba los clips generados.

---

## ⚙ ¿Cómo funciona?

1. _El usuario sube un video_

   - 🎥 Puede ser una clase, entrevista u otro material educativo.
   - El video se guarda en el servidor.

2. _La app transcribe el video con Whisper_

   - 🧠 Se genera la transcripción automática con timestamps (Whisper ya los genera por bloques).
   - Se muestra al usuario una lista de bloques con:

     - Texto parcial
     - Timestamp de inicio y fin  
       Ejemplo:

     00:00 → "Hola, bienvenidos al canal..."
     00:30 → "Hoy vamos a hablar sobre ansiedad..."
     01:00 → "La primera pregunta es..."

3. _El usuario elige los timestamps clave_

   - 🖱 Puede seleccionarlos desde la transcripción usando checkboxes, inputs o clics.
   - Ejemplo: [00:00, 00:30, 01:00, 02:15]

4. _La app corta el video automáticamente_

   - ✂ Con herramientas como _ffmpeg_, se fragmenta el video según los timestamps seleccionados.

5. _Se entregan los clips al usuario_
   - 📁 Cada clip se puede descargar individualmente.
   - Los nombres pueden sugerirse automáticamente: Tema1_Introduccion.mp4, Tema2_Ansiedad.mp4, etc.

---

## 👥 Posibles Usuarios

- Youtubers que suben entrevistas o cursos.
- Docentes que graban clases largas y desean dividirlas por capítulos.
- Periodistas que quieren segmentar sus notas o entrevistas.
- Creadores de podcast en video o audio que quieren cortar su contenido en secciones sin tener que editar todo manual

---

## 👥 Historias de Usuarios - TIMstamp para Docentes

Título: Dividir una clase larga en secciones temáticas

**Como** docente que graba clases completas para mis estudiantes,
**quiero** dividir fácilmente mis clases en capítulos temáticos,
**para** que mis alumnos puedan repasar por partes sin ver el video completo cada vez.

✅ Criterios de Aceptación
El docente puede subir un video largo de clase (3-5 hs.)

Se genera automáticamente la transcripción con bloques de texto y timstamps.

El docente puede marcar dónde empieza cada nuevo tema o capítulo con los timstamps que le da la aplicacion de ususario

Se generan clips individuales por cada sección marcada.

Cada clip puede tener un nombre sugerido como "Tema1_Introducción", "Tema2_Ejemplos", etc.

## 👥 Historia de Usuario - TIMstamp para YouTuber

**Como** YouTuber que subo entrevistas, podcasts y videos educativos de larga duración
**Quie**ro generar automáticamente capítulos con timestamps para mis videos
**Para** que mis suscriptores puedan saltar directamente a los temas que más les interesan, aumentar mi tiempo de visualización y mejorar el posicionamiento de mis videos en YouTube.

✅ Criterios de aceptación:

Puedo subir mi video grabado (MP4, MOV) o pegar el enlace de YouTube de un video ya publicado
El sistema identifica automáticamente los diferentes temas o secciones de mi contenido
Recibo una lista de capítulos sugeridos con:

Timestamp exacto (ej: 00:03:45)
Título descriptivo del tema (ej: "Consejos para principiantes")
Breve descripción opcional

Puedo personalizar los títulos y ajustar los tiempos antes de confirmar
Los capítulos se exportan en el formato exacto que necesito para la descripción de YouTube
Funciona con videos de 20 minutos a 3 horas de duración

## 🧰 Tecnologías y Herramientas a Utilizar

| Función                  | Herramienta                       |
| ------------------------ | --------------------------------- |
| Transcripción            | OpenAI Whisper API o modelo local |
| Backend                  | Python (Flask o FastAPI)          |
| Procesamiento de video   | FFmpeg                            |
| Control de versiones     | Git + GitHub                      |
| Organización del equipo  | GitHub Projects (Kanban)          |
| Frontend (posible)       | HTML + JS / React (opcional)      |
| Base de datos (opcional) | MySQL o SQLite                    |

---

## 🚀 Estado Actual

Estamos trabajando en el _Sprint 0_, que incluye:

- Definición y documentación del proyecto (README)
- Organización del equipo en GitHub
- Creación del Project Board y asignación de tareas iniciales
- Pruebas preliminares con transcripción automática

---

## 🧑‍💻 Integrantes del Equipo

<div>
  <h4>Integrantes</h4>
  <ul>
    <li>Juan Daniel Opazo</li>
    <li>Luciana Regina Varela</li>
    <li>Alejandra Elizabeth López</li>
    <li>Juan Manuel Yunes Mor</li>
  </ul>  
</div>

## 📁 Estructura Tentativa del Repositori

</div>
