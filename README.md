# Segundo Desempeño

Desarrollar una aplicación de gestión de una biblioteca. 
La aplicación debe permitir agregar, buscar y listar libros. 
Además, los datos de los libros deben ser cargados y guardados en un archivo CSV.

### Requisitos:

- Clase Libro:
Atributos: String titulo, String autor, int añoPublicacion, String isbn
Métodos: Constructores, getters, setters, toString()

- Clase Biblioteca:
Atributos: Map<String, Libro> libros (donde la clave es el ISBN del libro)
Métodos:
void agregarLibro(Libro libro)
Libro buscarLibroPorISBN(String isbn)
List<Libro> buscarLibrosPorAutor(String autor)
List<Libro> listarTodosLosLibros()
void cargarLibrosDesdeCSV(String nombreArchivo) throws IOException
void guardarLibrosEnCSV(String nombreArchivo) throws IOException

- Manejo de Excepciones:
Implementar manejo de excepciones adecuado para manejar errores de entrada/salida y casos donde el libro ya exista en la biblioteca.

- Archivo CSV:
Formato: titulo,autor,añoPublicacion,isbn


### Instrucciones
- Implementar la clase Libro.
- Implementar la clase Biblioteca con los métodos especificados.
- Implementar manejo de excepciones para los siguientes casos:
- Intento de agregar un libro con un ISBN que ya existe.
- Error al leer o escribir el archivo CSV.
- Desarrollar una clase principal que:
- Cree una instancia de Biblioteca.
- Cargue los libros desde un archivo CSV al inicio.
- Proporcione un menú para agregar, buscar y listar libros.
- Guarde los libros en un archivo CSV antes de salir.

## Puntaje
 - Clase Libro > Getters y Setters: 20p
 - Clase Bibioteca > buscarLibrosPorAutor: 10p
 - Clase Bibioteca > cargarLibrosDesdeCSV: 30p
 - Clase Bibioteca > guardarLibrosEnCSV: 30p
 - Compilacion general: 10p
