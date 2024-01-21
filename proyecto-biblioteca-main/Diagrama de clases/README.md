<div align = “justify">

# Diagrama-de-clases

## Diagrama
<img src = "../Imagenes/Diagrama de clases proyecto.jpg">

## Clases
Libro, Usuario, Préstamo, Biblioteca, EmpleadoBiblioteca, CategoriaLibro, Reserva, Editorial, Evento, Comentario.

## Atributos

|Clases|Atributos|
|---|---|
| Libro | ISBN, título, autor, año de publicación, cantidad de copias disponibles. |
| Usuario | Nombre, número de identificación, historial de préstamos. |
| Préstamo | Fecha de préstamo, fecha de devolución prevista, libro prestado, usuario que lo solicitó. |
| Biblioteca | Lista de libros disponibles, lista de usuarios registrados, historial de préstamos. |
| EmpleadoBiblioteca | Nombre, número de empleado, horario laboral. |
| CategoriaLibro | Nombre de la categoría, descripción, lista de libros en la categoría. |
| Reserva | Usuario que hizo la reserva, libro reservado, fecha de vencimiento de la reserva. |
| Editorial| Nombre de la editorial, lista de libros publicados. |
| Evento | Nombre del evento, fecha, descripción, lista de libros relacionados con el evento. |
| Comentario | Usuario que hizo el comentario, libro comentado, texto del comentario. |


## Conexiones
|  Libro | Conexión | 
|---|---|
| Préstamo  | Es una relación uno a muchos (Un libro puede tener varios préstamos). |
| Comentarios  | Es una relación uno a muchos (Un libro puede tener varios comentarios).
| Editorial  | Es una relación muchos a uno (Un libro puede ser publicado por una editorial).
| CategoríaLibro | Es una relación muchos a muchos (Un libro puede pertenecer a varias categorías y una categoría puede tener varios libros).  |

| Usuario | Conexión |
|---|---|
| Préstamo | Es una relación de uno a muchos (Un usuario puede tener cvarios préstamos). |
| Comentario | Es una relación de uno a muchos (Un usuario puede escribir varios comentarios). |

|  Préstamo | Conexión | 
|---|---|
| Libro  | Es una relación muchos a uno (Varios préstamos pueden estar asociados con un libro). |
| Usuario  | Es una relación muchos a uno (Varios préstamos pueden estar relacionados con un usuario).

|  Biblioteca | Conexión | 
|---|---|
| Libros  | Es una relación uno a muchos (Una biblioteca contiene varios libros). |
| Usuario  | Es una relación uno a muchos (Una biblioteca tiene a varios usuarios registrados).|
| Reserva | Es una relación uno a muchos (Una biblioteca puede tener varias reservas). |

|  CategoríaLibro | Conexión | 
|---|---|
| Libros  | Es una relación muchos a muchos (Una categoría puede terner varios libros).|

|  Reserva | Conexión | 
|---|---|
| Biblioteca  | Es una relación muchos a uno (Varias reservas pueden estar relacionadas con una biblioteca).|
| Usuario  | Es una relación muchos a uno (Varias reservas pueden estar relacionadas con un usuario).|
| Libro  | Es una relación muchos a uno  (Varias reservas pueden estar relacionadas con un libro).|

|  Editorial | Conexión | 
|---|---|
| Libro  | Es una relación uno a muchos (Una editorial puede tener varios libros publicados).|

|  EmpleadoBiblioteca | Conexión | 
|---|---|
| Biblioteca | Es una relación muchos a uno (Varios empleados pueden trabajar en una biblioteca).|







</div>
