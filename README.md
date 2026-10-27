# Segregacion-de-Interfaz
PrincipioSegregacion de Interfaz de SOLID


Este principio se aplica dividiendo las interfaces grandes en varias más pequeñas y específicas, para que las clases no tengan que implementar métodos que no ocupan:

- Se crearon interfaces pequeñas y abstractas como `Enviable`, `Remplazable` y `Expirable`, en lugar de juntar todo en una sola clase pesada.
- Las clases concretas, como `Fisico` y `Digital`, heredan únicamente de las interfaces que realmente necesitan para su funcionamiento (por ejemplo, `Digital` implementa `Expirable` y `Fisico` implementa `Enviable` y `Remplazable`).

De esta manera logramos que ningún cliente o clase dependa de métodos que no utiliza.
