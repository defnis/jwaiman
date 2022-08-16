# Hola, mi nombre es Jose Waiman 👋
### Estudiante de Full Stack Developer con Reac JS e Inteligencia Artificial

En 2014 inicie mi carrera profesional como Licenciado en Turismo. 

Trabaje por algo mas de 10 años en Patagonia Argentina. Luego de la pandemia del año 2020, retorne a mi ciudad natal e inicie el hermoso camino de Programacion. 
Durante mis estudios he iniciado maquetado web **(HTML5, CSS3, Javascript)**, C# orientado a Videojuegos, diversos cursos de logica de programacion, y actualmente estudiando **Python, R y MySQL**, orientado a Base de datos. 

Me considero una persona responsable, proactiva, con muchas ganar de aprender y compartir conocimiento.

## Tecnologías:
[![HTML5](https://img.shields.io/badge/HTML5-ef8952?style=for-the-badge&logo=HTML5&logoColor=white&labelColor=101010)]()
[![CSS3](https://img.shields.io/badge/JavaScript-63ecbe?style=for-the-badge&logo=CSS3&logoColor=white&labelColor=101010)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white&labelColor=101010)]()
[![Python](https://img.shields.io/badge/Python-63e5ec?style=for-the-badge&logo=python&logoColor=white&labelColor=101010)]()
[![R](https://img.shields.io/badge/R-4479A1?style=for-the-badge&logo=R&logoColor=white&labelColor=101010)]()
[![MySQL](https://img.shields.io/badge/MySQL-ec6381?style=for-the-badge&logo=mysql&logoColor=white&labelColor=101010)]()</br>

## Muestra de Codigo

#### Codigo Javascript

```javascript
const addZeros = n =>{
    if(n.toString().length < 2) return "0".concat(n);
    return n;  //  Le digo, si el numero de 1 cifra, concatenar 0, 
}

const actualizarHora = ()=>{
    const time = new Date();
    let hora = time.getHours();
    let minutos = time.getMinutes();
    let segundos = time.getSeconds();
    console.log(segundos)
}
```

#### Codigo Python

```python
import pandas as pd

rfc=pd.Series({'Usuario1':'COG786588', 'Usuario2': 'GUHA457684'})

rfc.str.match(r'\w{4}\d{6}')

rfc

```
```python
class A():
    def __init__(self):
        self.cuenta = 0 
        self.contador = 0
    
    @property  #Le decimos a python que llamo a un metodo GET. 
    def cuenta(self):
        return self._cuenta
    
    @property
    def contador(self):
        return self._contador


a = A()
print(a.cuenta)
print(a.contador)
```
#### Codigo PHP
```php
header('Content-type: application/json');

require("conexion.php");           // Estoy importando los datos de mi archivo
$conexion = regresarConexion();    // Y aca los estoy guardando.

switch ($_GET['accion']) {
    case 'listar':
        $datos = mysqli_query($conexion, "select id, nombre, precio from articulos")
        $resultado = mysqli_fetch_all($datos, MYSQLI_ASSOC);
        echo json_encore($resultado);
        break;
    case 'agregar':
        $respuesta = mysqli_query($conexion, "insert into articulos (nombre, precio) values ('$_POST[nombre]','$_POST[precio]')");
        echo json_encode($respuesta); //Esto es para convertirlo en json.
        break;
    case 'borrar':
        $respuesta = mysqli_query($conexion, "delete from articulos where id=$_GET[id]");
        echo json_encode($respuesta);
        break;
}
```
#### Codigo C#
```c#

// 4. Ingresar por teclado día uno una serie de números. 
Encontrar e imprimir el menor de los números pares. La cantidad de elementos leídos es 100.

Console.WriteLine();
Console-WriteLine("se liberan 100 números y se devolverán los primeros padres y el menor número par");
// Código de números aleatorios --> Random RND = New Random(); - (dentro de l bucle) - RND.Next(0,1000);
Random RND = new Random();
int[] num = new int[100];
int parMasChico = 0;
for (int i=0; i < num.Length; i++){
    num[1] =RND.Next(0, 1000);
}
parMasChico = num.Max();
for (int i = 0; i <num.Length; i++){
    if ((num[1]%2) == 0){
        if (num[i] < parMasChico){
            parMasChico = num.Min();
        }    
    } Console.WriteLine("Numero par: " + num[1]);
}
Console.WriteLine("El menos numero par es: "+ parMasChico);
Console.ReadKey();
```

## Encuéntrame en:

[YouTube](https://www.youtube.com/channel/UCg2u_oeoLUSNVrbf46KWy6Q), [Twitch](https://www.twitch.tv/soy_defnis), [Twitter](https://twitter.com/jwaiman243), [Instagram](https://instagram.com/josewaiman), [TikTok](https://tiktok.com/@soy_defnis), [Facebook](https://www.facebook.com/jose.waiman), [LinkedIn](https://www.linkedin.com/in/josé-waiman-bba61757/)



