1. ¿Hizo falta una base de datos real para probar la regla de negocio? ¿Qué dice eso sobre para qué sirve el patrón Repository?
No hizo falta por que los datos estaban guardados en un Map y el patron Repository los sacaba de ahi.

2. El Service recibe el repositorio como Repository<Prestamo>, no InMemoryPrestamoRepository. ¿Qué se rompía si usaban la clase concreta?
Si se usaba la clase InMemoryPrestamoRepository, el codigo se rompia por que el Service se iba a quedar acoplado a usar siempre la memoria.

3. Si cambiaran el Map en memoria por una base de datos real, ¿cuántos archivos tocarían? ¿Por qué tan pocos?
Muy pocos, por que el Service y el resto del sistema usan la interfaz, así que no les importa dónde ni cómo se guardan realmente los datos.