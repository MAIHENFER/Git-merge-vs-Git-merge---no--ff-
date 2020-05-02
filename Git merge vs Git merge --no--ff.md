## **Diferencias entre git merge y git merge --no--ff**

### **Git merge:**
* Realiza una fucion a tres bandas entre las 2 ultimas instantaneas de cada rama y el ancestro comun de ambas, creando un nuevo commit con los cambios mezclados.
* Con el git merge a la hora de unir necesitaremos hacer un commit mas, muchas veces llamado commit basura, ya que solamente se le añade un comentario.

### **Git merge --no--ff**
* Evita que ***git merge*** ejecute un avance rapido si detecta que se Head actual es un antecesor de la confirmacion que esta intentando fusionar, y siempre se creara un nuevo objeto de confirmacion.
* Esta combinacion de avance rapido puede ocurrir solemente cuando hay una ruta lineal desde la rama actual hasta la rama de destino
