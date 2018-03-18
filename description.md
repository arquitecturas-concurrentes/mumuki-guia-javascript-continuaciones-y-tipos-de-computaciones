Resulta bastante evidente que razonar sobre CPS es más complejo que en el estilo directo. Entonces, ¿por qué habríamos de adoptarlo?

CPS, al otorgarle a la función no sólo capacidad de cómputo sino de control, permite hacer cosas muy poderosas. En el caso que estudiamos anteriormente....

```
function succesor(x, cont) {
 cont(x + 1);
}
```

...no parece que estemos ganando mucho, porque la computación succesor puede ser modelada con una función con un sólo resultado posible. 

Pero sin embargo, podríamos haber aplicado a la función `cont` _cero o una vez_, o _cero o muchas veces_, podríamos haber recibido _múltiples continuaciones y ejecutar alguna de ellas_, o podríamos _haberlas ejecutado en otro momento_. CPS nos permite, entones, implementar 4 tipos de computaciones: con falla, no determinísticas, con excepciones y asincrónicas. ¡Aprendamos más sobre ellas!

