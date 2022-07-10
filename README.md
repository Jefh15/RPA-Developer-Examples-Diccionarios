# RPA-Developer-Examples-Diccionarios

Recapitulemos las actividades y los métodos utilizados

Comenzamos el proyecto como Secuencia creamos un nuevo Diccionario (String, String) para almacenar los nombres y las fechas de nacimiento (denominadas "FechasDeNacimiento");

Usamos 3 actividades Asignar para agregar elementos a la variable de diccionario: birthDates("key") = “value”. Las claves eran nombres y los valores eran fechas (dd/mm/aaaa);

Usamos una actividad Para cada para recorrer las claves de los Diccionarios y:

* Convertiremos cada valor en la fecha utilizando el método DateTime.Parse(birthDates(item)) y lo asignaremos a una variable recién creada DateTime (“fechaActual”);

* Determinaremos el cumpleaños del año actual mediante la expresión new DateTime(DateTime.Today.Year, dateCurrent.Month, dateCurrent.Day) y lo guardaremos en una variable recién creada DateTime ("CumpleañosDeEsteAño");

* Determinaremos el día de la semana del cumpleaños del año actual mediante la expresión currentYearAnniversary.DayOfWeek.ToString y lo guardaremos en una variable recién creada Cadena ("DíaSemanaCumpleaños");

* Usaremos una actividad Si para verificar si el cumpleaños del año actual ha pasado por la condición "CumpleañosDeEsteAño < DateTime.Today":

* Si es True, utilizaremos una actividad Registrar mensaje para imprimir que el cumpleaños de esa persona pasó y el día de la semana en que cayó;

* Si es False, utilizaremos una actividad Registrar mensaje para imprimir que el cumpleaños de esa persona será en el futuro y el día de la semana en el que será.