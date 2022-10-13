# Activitat 2 - Pràctica amb llenguatges

## Grup: Javier Mouriño y Byron Cobos

### Per al llenguatge compilat: C++

**Utilitzant la línia de comandes, sense utilitzar un IDE de desenvolupament escriureu el programa en un fitxer de text que sigui el codi font, el codi font l’adjunteu dins el document.**

```

#include <iostream>
#include <cstdlib>
#include "time.h"

int Droll()
{
    int outcome;
    int l_limit = 1;  // floor or lower limit of a die
    int h_limit = 6; //ceiling or higher limit of a die

    outcome = rand() % (h_limit - l_limit + 1) + l_limit;

    return outcome;
}

int main()
{
    srand(time(0));
    for(int i=0;i<1;i++)
    {
        std::cout << Droll() << std::endl;
    }
}

```

Instalará el **compilador GCC** altres eines de desenvolupament.
“La GNU Compiler Collection és un conjunt de recopiladors de llenguatges de programació creat pel Projecte GNU. Així doncs, és programari lliure distribuït per la Free Software Foundation sota la llicència GNU General Public License”

![image](https://user-images.githubusercontent.com/113586156/195358732-f27ef4e6-0062-45dc-aeab-ae851906e2b6.png)

**Identifiqueu el compilador real que utilitzeu (nom de l’executable) i la comanda per utilitzar-lo per passar de codi font a codi objecte.** 

![image](https://user-images.githubusercontent.com/113586156/195361555-0333f24b-6b38-4377-97f0-b8402b4f9d2c.png)

**Descriviu com passar de codi font a codi objecte.** 

Al terminal executem la comanda nano per obrir un editor de text a la mateixa consola, on hi guardarem el nostre codi font (.txt) en objecte (.cpp) .
 
**Mostreu les extensions dels fitxers de codi font i codi objecte.**

![image](https://user-images.githubusercontent.com/113586156/195370216-a6c9c5b5-0604-402d-b4c6-5defc53ab09c.png)

.txt i .cpp

**Descriviu com passar de codi objecte a executable.**

![image](https://user-images.githubusercontent.com/113586156/195362055-de5f0b9b-dced-45ed-bc20-a455eb6a2eec.png)

Utilizem les comandes g++ -o d6 d6.cpp (d6.cpp --> es el nostre codi objecte)(d6 --> serà el nostre .exe)

**Expliqueu els avantatges d’utilitzar un llenguatge compilat i els punts febles.**

Avantatge: conté un rang de dades bastant ampli.

Punts febles: que necessita molts de recursos per executar-se.

**Busqueu 3 IDEs de desenvolupament pel llenguatge.**

Microsft Visual C++

Borland C++

IDE Eclipse

**Webgrafia**

https://hetpro-store.com/TUTORIALES/compilar-cpp-g-linux-en-terminal-leccion-1/

https://www.delftstack.com/es/howto/cpp/cpp-dice-roll/

https://www.onlinegdb.com/fork/H1TLQdVSU

https://ca.wikipedia.org/wiki/GNU_Compiler_Collection

https://ca.myservername.com/top-22-online-c-compiler-tools-best-c-ide

============================================================================================================

### Per al llenguatge interpretat: Python

**Utilitzant la línia de comandes, sense utilitzar un IDE de desenvolupament escriureu el programa en un fitxer de text que sigui el codi font, el codi font l’adjunteu dins el document.**

```

import random

while True:
    resultado = random.randint(1,6)
    print("El dado giro y obtuvo: ", resultado)
    input("Presiona cualquier tecla para lanzar nuevamente.")
    
```     

**Identifiqueu l'intèrpret del llenguatge (l’executable).**

![image](https://user-images.githubusercontent.com/113586156/195454764-edfe29c6-bc82-4b66-b013-1e81622061e2.png)

python3 d6.py

**Descriviu com funciona l’intèrpret.**

![image](https://user-images.githubusercontent.com/113586156/195454083-946b9c9a-a11d-4699-9c1a-881f153eca15.png)

Executa el programa, fins que l'usuari vulgui. 

**Mostreu les extensions dels fitxers de codi font.**

![image](https://user-images.githubusercontent.com/113586156/195453970-57653db5-dd5b-48b9-b2af-19535abbe16f.png)

**Expliqueu els avantatges d’utilitzar un llenguatge interpretat i els punts febles.** 

Avantatges: no necessita ser compilat, es sencill i rápid, flexible.

Punts febles: l'execució d'aquests llenguatges és més lenta a diferència dels llenguatges compilats, són difícils de depurar.

**Busqueu 3 IDEs de desenvolupament pel llenguatge.**

PyCharm

KDevelop

SlickEdit

**Webgrafia**

http://copitosystem.com/es/python-dice-simulator/

https://ajaxhispano.com/ask/que-uso-en-linux-para-hacer-ejecutable-un-programa-python-25213/

https://ca.eyewated.com/diferencia-entre-llenguatges-compilats-i-interpretats/


============================================================================================================

### Per al llenguatge de MV: Java

**Utilitzant la línia de comandes, sense utilitzar un IDE de desenvolupament escriureu el programa en un fitxer de text que sigui el codi font, el codi font l’adjunteu dins el document.**

```

public class Dado6Caras {
   public static void main(String[] args) {
      /* Math.random() * 6 + 1
       int ValorDado = Math.floor(Math.random()*6+1);
       int ValorEntero = Math.floor(Math.random()*(N-M+1)+M);*/

       Random r = new Random();
       int d6 = r.nextInt(6) + 1;
       System.out.println(d6);
   }
}

```

![image](https://user-images.githubusercontent.com/113586156/195460161-34a51288-0730-418d-9928-3312145b39a2.png)

![image](https://user-images.githubusercontent.com/113586156/195460259-395492a3-938e-4247-833c-fab1531162b4.png)

Realitzem l'instal·lació del compilador de Java.

**Identifiqueu el compilador real (nom d’executable) que utilitzeu i la comanda per utilitzar-lo per passar de codi font a ByteCode.**

d6.java ----> nano, guardem el codi font i el guardem .java

**Descriviu com passar de codi font a ByteCode.** 

![image](https://user-images.githubusercontent.com/113586156/195462403-bac5ddc7-e201-49f7-a705-f4e758d928dc.png)

javac d6.java i em crea la classe d6.class , per poder executar conjuntament.

**Mostreu les extensions dels fitxers de codi font i ByteCode.**

![image](https://user-images.githubusercontent.com/113586156/195462677-9c8f5581-7dff-4742-9d89-b5b35490ffac.png)

**Descriviu com executar el programa.**

![image](https://user-images.githubusercontent.com/113586156/195462718-60c5c284-8238-4433-9dd2-645e38394163.png)

Executem la comanda java d6.java (perque ja està compilat), i fem ús fins que l'usuari vulgui.

**Expliqueu els avantatges d’utilitzar un llenguatge de MV i els punts febles.**

Pros:

L’intèrpret sol estar en més d’un sistema operatiu així que no cal adaptar el seu codi a una plataforma en concret.

El programa es pot portar en diferents plataformes.

El rendiment és superior respecte als llenguatges compilats.

Contres:

Velocitat de processament més lenta respecte als llenguatges compilats.

El codi font pot ser modificat per qualsevol persona que tingui accés a ell.

Per a executar el codi sempre fa falta un intèrpret.

**Busqueu 3 IDEs de desenvolupament pel llenguatge.**

Visual Studio

Eclipse

Intellij IDEA

**Webgrafia**

https://open-bootcamp.com/aprender-programar/lenguaje-interpretado 

https://www.softzone.es/programas/lenguajes/mejores-ide-programar/

https://www.java.com/es/download/help/enable_panel.html

https://aprendiendoaprogramar.es/blog/ventajas-y-desventajas-de-la-maquina-virtual/

https://www.adslzone.net/listas/mejores-programas/maquinas-virtuales/
