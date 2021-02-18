# Web Developer
>C ++ is one of the first programming languages that I learned in university, especially in the subject of algorithms and data structures. Next you will see a mini program in this language.
#### C++
```c++
#include <iostream>
#include<stdlib.h>
#include <cstring>

using std :: cout;
using std :: cin;
using std :: endl;

#define _CANTEST 2

typedef char str10[10];
typedef char str15[20];
typedef char str20[30];

struct tRegEstudiante{
  str10 nombre;
  str15 apellido;
  str20 carrera;

}; 

typedef tRegEstudiante tVecEst[_CANTEST];

void inicializarVecEst(tVecEst, int);
void ingresarEst(tVecEst, int);
void mostrarEst(tVecEst, int);
int main() {

  tVecEst v;
  int cant;
  cant = _CANTEST;

  inicializarVecEst(v,cant);
  ingresarEst(v,cant);
  mostrarEst(v, cant);

}
void inicializarVecEst(tVecEst v, int cant){
  for(int i = 0; i < cant; i++){
    strcpy(v[i].nombre, "");
    strcpy(v[i].apellido, "");
    strcpy(v[i].carrera, "");
  }
}
void ingresarEst(tVecEst v, int cant){
  cout<<"Ingrese estudiante"<<endl;
  cout<<"=================="<<endl;
  
  for(int i = 0; i < cant; i++){
    cout<<"Nombre: ";
    cin.getline(v[i].nombre,sizeof(v[i].nombre),'\n');
    cout<<"Apellido: ";
    cin.getline(v[i].apellido,sizeof(v[i].apellido),'\n');
    cout<<"Carrera: ";
    cin.getline(v[i].carrera,sizeof(v[i].carrera),'\n');
    cout<<"----------------------------"<<endl;
  }
}
void mostrarEst(tVecEst v , int cant){
  cout<<"========================================"<<endl;
  cout<<"   NOMBRE   "<<"  APELLIDO   "<<"  CARRERA  "<<endl;
  cout<<"========================================"<<endl;
  for(int j = 0; j < _CANTEST; j++ ){
  cout<<"\t"<<v[j].nombre<<"\t\t"<<v[j].apellido<<"\t\t"<<v[j].carrera<<endl;
  }
}
  
  }
```
---
#### JS
```javascript
  console.log('I am Web Developer');
```

- 👋 Hi, I’m Aldo Ruiz a Web Developer.
- 👀 I’m interested in Web and Mobile Develope.
- 🌱 I’m currently learning Angular, Vue and React.
 

<!---
DVs07/DVs07 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
