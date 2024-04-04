 # Examen Práctico de Recuperación U1

 ## Gestión de cursos universitarios.


### Instrucciones:

Este examen práctico tiene como objetivo evaluar tus habilidades en la programación Orientada a Objetos (POO) para desarrollar un sistema de gestión de cursos universitarios.
Deberás implementar el sistema utilizando los conceptos y técnicas de la POO.
No se permite el uso de internet ni de ningún otro material de apoyo durante el examen.


### Descripción del sistema:

Se deberá generar un sistema en java/maven que te gestione cursos universitarios, cada curso se denomina "Grupo", cada grupo tiene asignado un profesor, un horario, una materia y un grupo de alumnos. La materia tiene nombre de la materia, horas semanales y número de créditos. El horario son las horas y días de la semana que se impartirá el curso/materia. Cada alumno tiene su nombre, matrícula, grado. Se gestionan las calificaciones de los alumnos en el grupo para obtener su promedio en el grupo. Como salida genera el enunciado detallado, además genera una descripción para cada clase del sistema.

El sistema debe gestionar los siguientes elementos:

Grupos: Cada curso se denomina "Grupo" y tiene las siguientes características:

Nombre: Nombre del curso (de tipo String)
Profesor: Profesor asignado al curso (de tipo Profesor)
Horario: Horario del curso (de tipo Horario)
Materia: Materia del curso (de tipo Materia)
Alumnos: Lista de alumnos matriculados en el curso
Materias: Cada materia tiene las siguientes características:

Nombre: Nombre de la materia (de tipo String)
HorasSemanales: Horas semanales de la materia (de tipo int)
Creditos: Número de créditos de la materia (de tipo int)
Horario: El horario del curso tiene las siguientes características:

Dias: Días de la semana en que se imparte el curso 
Horas: Horas en que se imparte el curso
Alumnos: Cada alumno tiene las siguientes características:

Nombre: Nombre del alumno (de tipo String)
Matricula: Matrícula del alumno (de tipo String)
Grado: Grado del alumno (de tipo String)
Calificaciones: El sistema debe gestionar las calificaciones de los alumnos en cada grupo. Se debe calcular el promedio de cada alumno en cada grupo.

### Salida:

El sistema debe generar la siguiente salida:

Listado de grupos con la siguiente información:

Nombre del grupo
Nombre del profesor
Horario del grupo
Materia del grupo
Lista de alumnos matriculados en el grupo
Listado de alumnos con la siguiente información:

Nombre del alumno
Matrícula del alumno
Grado del alumno
Promedio del alumno en cada grupo
Clases del sistema:

Clase Grupo:

Atributos:
nombre: Nombre del grupo (de tipo String)
profesor: Profesor asignado al curso (de tipo Profesor)
horario: Horario del curso (de tipo Horario)
materia: Materia del curso (de tipo Materia)
alumnos: Lista de alumnos matriculados en el curso (de tipo List<Alumno>)
Métodos:
Constructor que inicializa los atributos del grupo.
Métodos get y set para cada atributo.
Método addAlumno() que añade un alumno a la lista de alumnos del grupo.
Método removeAlumno() que elimina un alumno de la lista de alumnos del grupo.
Método getPromedioAlumno() que calcula el promedio de un alumno en el grupo.

Clase Profesor:

Atributos:
nombre: Nombre del profesor (de tipo String)
especialidad: Especialidad del profesor (de tipo String)
Métodos:
Constructor que inicializa los atributos del profesor.
Métodos get y set para cada atributo.

Clase Horario:

Atributos:
dias: Días de la semana en que se imparte el curso (de tipo List<String>)
horas: Horas en que se imparte el curso (de tipo List<String>)
Métodos:
Constructor que inicializa los atributos del horario.
Métodos get y set para cada atributo.

Clase Materia:

Atributos:
nombre: Nombre de la materia (de tipo String)
horasSemanales: Horas semanales de la materia (de tipo int)
creditos: Número de créditos de la materia
número de unidades

### Entregables

Se deberá generar un sistema capaz de realizar la gestión  (CRUD) de alumnos que tomarán el curso, agregar profesor al curso, asignar materia al grupo. Así como la asignación de calificaciones de las unidades para obtener el promedio del grupo y de cada alumno.