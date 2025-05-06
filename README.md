# Ejercicio: Sistema de Biblioteca (Diagrama ER)

Imagina una pequeña biblioteca que quiere registrar información básica sobre los libros, los socios (personas que piden libros prestados) y los préstamos.

## Requisitos
1. La biblioteca tiene muchos **libros**, y de cada libro se quiere guardar:
   - ID del libro
   - Título
   - Autor
   - Año de publicación
2. La biblioteca tiene varios **socios**, de los cuales se guarda:
   - ID del socio
   - Nombre
   - Fecha de registro
3. Cada socio puede pedir prestado varios libros, y cada libro puede ser prestado muchas veces (a diferentes socios). Por cada **préstamo** se quiere registrar:
   - Fecha del préstamo
   - Fecha de devolución (puede estar vacía si el libro aún no ha sido devuelto)
## Tarea
1. Identifica las **entidades**, sus **atributos** y las **relaciones** entre ellas.
2. Dibuja el **diagrama ER** con:
   - Entidades (rectángulos)
   - Atributos (óvalos)
   - Relaciones (rombos)
   - Cardinalidad (por ejemplo: uno a muchos, muchos a muchos)
## Entidades sugeridas
- **Libro**
  - ID_Libro (PK)
  - Título
  - Autor
  - Año_Publicación
- **Socio**
  - ID_Socio (PK)
  - Nombre
  - Fecha_Registro
- **Préstamo**
  - Fecha_Préstamo
  - Fecha_Devolución
## Relaciones sugeridas
- Un **Socio** puede tener muchos **Préstamos**
- Un **Libro** puede estar en muchos **Préstamos**
- La relación entre **Socio** y **Libro** es **muchos a muchos** a través de **Préstamo**
