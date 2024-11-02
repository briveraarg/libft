## Mi libft

Este es el primer proyecto como estudiante de 42. Debemos programar algunas funciones de la librería estándar de C, así como otras funciones que te serán útiles a lo largo de todo el cursus. Sos oficialmente un estudiante de 42 cuando pasas tu libft.

---

### *Parte obligatoria del proyecto*

### Funciones estándar de C

Las funciones de manipulación y verificación de cadenas y memoria son fundamentales en la programación en C. Algunas de las más importantes incluyen:

- [ft_isalpha](https://github.com/briveraarg/libft/blob/main/ft_isalpha.c)
- [ft_isdigit](https://github.com/briveraarg/libft/blob/main/ft_isdigit.c)
- [ft_isalnum](https://github.com/briveraarg/libft/blob/main/ft_isalnum.c)
- [ft_isascii](https://github.com/briveraarg/libft/blob/main/ft_isascii.c)
- [ft_isprint](https://github.com/briveraarg/libft/blob/main/ft_isprint.c)

Estas funciones permiten verificar tipos de caracteres, mientras que [ft_strlen](https://github.com/briveraarg/libft/blob/main/ft_strlen.c) mide la longitud de una cadena. Para la gestión de memoria, utilizamos:

- [ft_memset](https://github.com/briveraarg/libft/blob/main/ft_memset.c)
- [ft_bzero](https://github.com/briveraarg/libft/blob/main/ft_bzero.c)

Además, [ft_memcpy](https://github.com/briveraarg/libft/blob/main/ft_memcpy.c) y [ft_memmove](https://github.com/briveraarg/libft/blob/main/ft_memmove.c) manejan la copia de datos. Otras funciones útiles incluyen:

- [ft_strlcpy](https://github.com/briveraarg/libft/blob/main/ft_strlcpy.c)
- [ft_strlcat](https://github.com/briveraarg/libft/blob/main/ft_strlcat.c)
- [ft_toupper](https://github.com/briveraarg/libft/blob/main/ft_toupper.c)
- [ft_tolower](https://github.com/briveraarg/libft/blob/main/ft_tolower.c)

Las funciones de búsqueda y comparación como:

- [ft_strchr](https://github.com/briveraarg/libft/blob/main/ft_strchr.c)
- [ft_strrchr](https://github.com/briveraarg/libft/blob/main/ft_strrchr.c)
- [ft_strncmp](https://github.com/briveraarg/libft/blob/main/ft_strncmp.c)
- [ft_memchr](https://github.com/briveraarg/libft/blob/main/ft_memchr.c)
- [ft_memcmp](https://github.com/briveraarg/libft/blob/main/ft_memcmp.c)

son esenciales para la comparación de datos. Por último, [ft_strnstr](https://github.com/briveraarg/libft/blob/main/ft_strnstr.c) busca subcadenas y [ft_atoi](https://github.com/briveraarg/libft/blob/main/ft_atoi.c) convierte cadenas a enteros. Para implementar las funciones [ft_calloc](https://github.com/briveraarg/libft/blob/main/ft_calloc.c) y [ft_strdup](https://github.com/briveraarg/libft/blob/main/ft_strdup.c), se requiere el uso de `malloc()` para la asignación dinámica de memoria.

---

### Otras funciones

En esta segunda parte del proyecto, se desarrollará un conjunto de funciones que, aunque pueden estar presentes en la librería libc, se implementarán de manera diferente. Entre las funciones a crear se encuentran:

- **[ft_substr](https://github.com/briveraarg/libft/blob/main/ft_substr.c)**: permite reservar y devolver una substring de la cadena `s`, comenzando desde el índice `start` y con una longitud máxima `len`, devolviendo NULL si falla la reserva de memoria.
  
- **[ft_strjoin](https://github.com/briveraarg/libft/blob/main/ft_strjoin.c)**: concatena las cadenas `s1` y `s2`, reservando memoria con `malloc()`.

- **[ft_strtrim](https://github.com/briveraarg/libft/blob/main/ft_strtrim.c)**: elimina caracteres de la cadena `set` desde el principio y el final de `s1`, devolviendo la cadena recortada.

- **[ft_split](https://github.com/briveraarg/libft/blob/main/ft_split.c)**: separa una cadena en substrings utilizando un carácter delimitador `c`.

- **[ft_itoa](https://github.com/briveraarg/libft/blob/main/ft_itoa.c)**: convierte un entero `n` a su representación en string, manejando correctamente los números negativos.

- **[ft_strmapi](https://github.com/briveraarg/libft/blob/main/ft_strmapi.c)** y **[ft_striteri](https://github.com/briveraarg/libft/blob/main/ft_striteri.c)**: aplican una función a cada carácter de una cadena, generando una nueva cadena o modificando la original, respectivamente.

Finalmente, se implementarán funciones para la salida de caracteres y strings a un file descriptor, como:

- [ft_putchar_fd](https://github.com/briveraarg/libft/blob/main/ft_putchar_fd.c)
- [ft_putstr_fd](https://github.com/briveraarg/libft/blob/main/ft_putstr_fd.c)
- [ft_putendl_fd](https://github.com/briveraarg/libft/blob/main/ft_putendl_fd.c)
- [ft_putnbr_fd](https://github.com/briveraarg/libft/blob/main/ft_putnbr_fd.c)

Todas estas funciones utilizan la función `write` para realizar la escritura.

---

### Bonus

En la parte bonus del proyecto, se abordará la manipulación de listas mediante la creación de una estructura de nodo, `t_list`, que contiene un puntero a su contenido y otro puntero al siguiente nodo. Se recomienda añadir esta estructura al archivo [libft.h](https://github.com/briveraarg/libft/blob/main/libft.h). Las funciones que se implementarán para gestionar estas listas son diversas:

- **[ft_lstnew](https://github.com/briveraarg/libft/blob/main/ft_lstnew.c)**: crea un nuevo nodo y asigna su contenido utilizando `malloc()`.

- **[ft_lstadd_front](https://github.com/briveraarg/libft/blob/main/ft_lstadd_front.c)**: añade un nodo al inicio de la lista.

- **[ft_lstsize](https://github.com/briveraarg/libft/blob/main/ft_lstsize.c)**: cuenta el número de nodos presentes.

- **[ft_lstlast](https://github.com/briveraarg/libft/blob/main/ft_lstlast.c)**: accede al último nodo de la lista.

- **[ft_lstadd_back](https://github.com/briveraarg/libft/blob/main/ft_lstadd_back.c)**: permite añadir un nodo al final de la lista.

- **[ft_lstdelone](https://github.com/briveraarg/libft/blob/main/ft_lstdelone.c)**: libera un nodo específico y su contenido.

- **[ft_lstclear](https://github.com/briveraarg/libft/blob/main/ft_lstclear.c)**: libera un nodo y todos los nodos consecutivos, asegurándose de que el puntero a la lista sea NULL al finalizar.

- **[ft_lstiter](https://github.com/briveraarg/libft/blob/main/ft_lstiter.c)**: aplica una función a cada nodo.

- **[ft_lstmap](https://github.com/briveraarg/libft/blob/main/ft_lstmap.c)**: crea una nueva lista aplicando una función a cada nodo de la lista original, utilizando otra función para gestionar la liberación de contenido si es necesario.

Para que la evaluación de esta parte bonus se lleve a cabo, es crucial que la parte obligatoria esté completa y sin errores.
