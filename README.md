# Proyecto-II

# Equipo
- Froylan Adair Villegas Castro
- Diego Juan Manuel Salvador Garcia Reyna
- Hector Alejandro Perez Cornejo
- Isay Montejano Quirino
- Cesar Mocivais Aguilar
- Daniel Rodriguez Burnes
- Maximiliano Lugo Zabala
- Aurelio Flores Nava
# Sistema de Gestión Académica

Este proyecto es un sistema de gestión académica desarrollado con FastAPI, MongoDB y AWS S3. Permite gestionar alumnos, profesores, materias, calificaciones e inscripciones, así como manejar la autenticación de usuarios mediante JWT (JSON Web Tokens).

## Descripción

El sistema permite realizar las siguientes operaciones:

- **Gestión de Alumnos**: Crear, leer, actualizar y eliminar registros de alumnos, así como subir imágenes de perfil a AWS S3.
- **Gestión de Profesores**: Crear, leer, actualizar y eliminar registros de profesores.
- **Gestión de Materias**: Crear, leer, actualizar y eliminar materias, así como asignar materias a profesores.
- **Gestión de Calificaciones**: Registrar y consultar calificaciones de alumnos por materia.
- **Gestión de Inscripciones**: Inscribir alumnos en materias y consultar inscripciones.

## Requisitos

- Python 3.7 o superior
- MongoDB
- AWS S3 (para almacenamiento de imágenes)

# Autenticación
- POST /token: Obtiene un token JWT al proporcionar un nombre de usuario y una contraseña.
# Alumnos
- GET /alumnos/: Obtiene todos los alumnos.
- GET /alumnos/{alumno_id}: Obtiene un alumno por su ID.
- POST /alumnos/: Crea un nuevo alumno (puede incluir una imagen).
- PUT /alumnos/{alumno_id}: Actualiza la información de un alumno.
- DELETE /alumnos/{alumno_id}: Elimina un alumno.
# Profesores
- GET /profesores/: Obtiene todos los profesores.
- GET /profesores/{profesor_id}: Obtiene un profesor por su ID.
- POST /profesores/: Crea un nuevo profesor.
- PUT /profesores/{profesor_id}: Actualiza la información de un profesor.
- DELETE /profesores/{profesor_id}: Elimina un profesor.
# Materias
- GET /materias/: Obtiene todas las materias.
- GET /materias/{materia_id}: Obtiene una materia por su ID.
- POST /materias/: Crea una nueva materia.
- PUT /materias/{materia_id}: Actualiza la información de una materia.
- DELETE /materias/{materia_id}: Elimina una materia.
- POST /materias/asignar/: Asigna una materia a un profesor.
# Calificaciones
- GET /calificaciones/alumno/{alumno_id}: Obtiene las calificaciones de un alumno.
- GET /calificaciones/materia/{materia_id}: Obtiene las calificaciones de una materia.
- POST /calificaciones/: Agrega una nueva calificación.
# Inscripciones
- GET /inscripciones/alumno/{alumno_id}: Obtiene las inscripciones de un alumno.
- POST /inscripciones/: Inscribe a un alumno en una materia.
- DELETE /inscripciones/{inscripcion_id}: Elimina una inscripción.
