# Programación de una primer versión de DApp  por Alberto López Gutiérrez

Este es mi primer proyecto de DApp y tiene mucho tiempo que no programo, así que estoy muy emocionado por esto. Comencemos.

NOTA: Desde que inicié este master, no ha existido un grupo, siempre hemos entregado mis compañeros y yo el trabajo de forma individual, me parece que sólo ha habido un grupo. En mi caso continuaré con la entrega individual. Muchas gracias!!

## Sprint 2

Lo siguiente fue desplegado en un Ubuntu LTS 22.04, lo primero que hice fue instalar Node.js en el ubuntu, recurrí directamente a las herramientas de Ubuntu (APT) donde instale nodejs y también npm, se puede verificar su versión. Ocupé el blog de [Edward S. & Aris B.](https://www.hostinger.com/tutorials/how-to-install-node-ubuntu?ppc_campaign=google_search_generic_hosting_all&bidkw=defaultkeyword&lo=9047091&gad_source=1&gclid=CjwKCAiAuYuvBhApEiwAzq_Yiay1MIqRX_uv-ElLgxUZHYyhim5ske-hRuoeqoNvAhFRWnORk975dhoCFjUQAvD_BwE) de Hostinger para realizar esta operación. Esta primer parte también viene del Sprint 1, a pesar de que fue teórico, realicé la parte del despliegue del Ganache, por medio del tutorial de [Diego Escalona](https://github.com/Diegoescalonaro/react-simple-truffle-box). Gracias Profesor!

Primero actualicé la máquina

![image](https://github.com/alopez2003/dapps1/assets/67942268/28a4a934-b168-4969-9757-c14f6bf7342d)

Posteriormente instalé Nodejs

![image](https://github.com/alopez2003/dapps1/assets/67942268/1237345e-b4a0-4e52-9257-10acab81827b)

Posteriormente instalé NPM

![image](https://github.com/alopez2003/dapps1/assets/67942268/acf49a07-5dd9-441e-9757-19ce78db115d)

Podemos ver las versiones de nodejs y npm, sin embargo son antiguas las que se encuentran en las librerias de Ubuntu 22.04

![image](https://github.com/alopez2003/dapps1/assets/67942268/697bc45c-153b-4eaa-bb85-1a40b63ec1ab)

Después bajamos e instalamos NVM

![image](https://github.com/alopez2003/dapps1/assets/67942268/af6dbbde-e10c-4b86-90f3-0d3f7bc0efc7)

Con esto logramos actualizar Nodejs

![image](https://github.com/alopez2003/dapps1/assets/67942268/fb15317e-b1be-46d3-9ff8-f26af566b4ae)

![image](https://github.com/alopez2003/dapps1/assets/67942268/1646084b-85ee-4b7b-9480-97044fc0495f)

![image](https://github.com/alopez2003/dapps1/assets/67942268/d0b3fef6-eec5-417c-b383-05dc0a68ddc7)

Para la actualización recurrimos a las siguientes ligas

[https://phoenixnap.com/kb/update-node-js-version](https://phoenixnap.com/kb/update-node-js-version)
[https://www.howtoforge.com/how-to-manage-nodejs-versions-with-n-in-ubuntu-20-04/](https://www.howtoforge.com/how-to-manage-nodejs-versions-with-n-in-ubuntu-20-04/)

Posteriormente creamos una cuenta de MetaMask en la máquina Ubuntu

![image](https://github.com/alopez2003/dapps1/assets/67942268/d9065465-e6cb-41bd-b534-f5aab5d47341)

De inicio, tiene la siguiente Address 0xFa61B9977887aC8A3A2d2ba86e7b46E3194Effe4, sin embargo estaremos trabajando con Ganache

Después creamos el directorio para la instalación de Truffle

![image](https://github.com/alopez2003/dapps1/assets/67942268/44d8f3b1-572b-4bab-bcb4-633d16d4fd3e)

![image](https://github.com/alopez2003/dapps1/assets/67942268/5ea1c746-3e60-4ca4-b226-dd79881f5db8)

Realizamos el unbox del compartido de Diego Escalona

![image](https://github.com/alopez2003/dapps1/assets/67942268/5cbd8278-2789-47dd-a83a-bfbb23e215f4)

Podemos ver el contenido ya en la carpeta

![image](https://github.com/alopez2003/dapps1/assets/67942268/79f75f31-9947-439f-839c-c2cd348fb7f2)

Cabe mencionar que el Smart Contract que ocuparemos para la verificación de integridad en la blockchain de un archivo lo tomamos modificando el archivo de [Auction.sol](https://github.com/Diegoescalonaro/auction-smartcontract/blob/master/Auction.sol), también de Diego Rodriguez.

El archivo se llama Integrity.sol, mismo que anexo en este repositorio.

Ejecutamos ganache 

![image](https://github.com/alopez2003/dapps1/assets/67942268/aad0cad5-e071-4647-96a9-d23d3ebd2aea)

![image](https://github.com/alopez2003/dapps1/assets/67942268/9422c092-61f1-4d9d-bcbb-a1c5661711d8)

![image](https://github.com/alopez2003/dapps1/assets/67942268/e5b92f6e-9731-4cb0-a5cf-f5927f293237)

Añadimos el archivo Integrity.sol a la carpeta de contratos

![image](https://github.com/alopez2003/dapps1/assets/67942268/7838a6b3-e20a-4bc9-993e-25d14c9faea2)

Modificamos el script de despliegue para que despliegue el contrato de Integrity

![image](https://github.com/alopez2003/dapps1/assets/67942268/08f2e242-3251-4ed1-b04e-90d0b8a147fb)

Modificamos el archivo truffle-config.js para que coincida el puerto de conexión de ganache, tenía el 8545 y está ejecutando sobre el 7545 con el network ID 5777

<![image](https://github.com/alopez2003/dapps1/assets/67942268/92be1aa9-91a6-470e-b5f9-ee7a1281bd13)
























