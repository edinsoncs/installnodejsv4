##Instalar Nodejs V.4 - Centos
**Primer paso**

wget http://people.centos.org/tru/devtools-2/devtools-2.repo -O /etc/yum.repos.d/devtools-2.repo

**Segundo paso**
Tuve algunos problemas al instalar, pero esta es la solución necesitamos nuestro compilador actualizado

yum install -y devtoolset-2-gcc devtoolset-2-binutils devtoolset-2-gcc-c++

**Tercer paso**

scl enable devtoolset-2 bash

**Cuarto paso**
En este paso agregaremos nuestra url de nodejs

wget https://nodejs.org/dist/v4.1.2/node-v4.1.2.tar.gz 

**Quinto paso**
Si es tu primera ves instalando nodejs en produccion, te saldran varios numeros indicando la descarga, una ves completado escribe **ls** para ver si se descargo correctamente

Escribiremos lo siguiente, esto desempaquetara nuestri node.tar.gz

tar -zxvf node-v4.1.2.tar.gz

**Sexto paso**
Ingresamos a nuestro folder

cd node-v4.1.2.tar.gz

**Septimo paso**
Escribimos lo siguiente:

./configure

**Octavo paso**
make

**Noveno paso**
make install 

**Decimo paso**
Escribimos node -v

**Finish** 



