**Usando máscaras, escriba las instrucciones necesarias para hacer que los primeros 4 pines del puerto C sean entradas, y los 4 últimos sean salidas. De los pines configurados como salida, dos cualesquiera estarán altos, y dos bajos.**

```c++

void main (void){
    TRISC |= 0X0F;//Puertos de Entrada
    TRISC &= ~0XF0;//Puertos de Salida
    PORTB |= 0X03;//Pines en Alto
    PORTB &= ~0X0C;//Pines en Bajo
}
```

