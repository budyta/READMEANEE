# Trabajo REMIX 

## **Remix**
Remix (también conocido como Browser-Solidity) es un compilador de Solidity basado en navegador e IDE.
Visite [https://remix.ethereum.org](google.es) para usar; siempre entregará la última versión  

## **Uso Offline**
La rama gh-pages siempre tiene la última versión estable de Remix. También contiene un archivo ZIP con toda la compilación. Descárguelo para usar sin conexión.
Nota: contiene la última versión de Solidez disponible en el momento del embalaje. No se admiten otras versiones de compilador.  

## **INSTALACIÓN:**  
Instale npm y node.js (consulte [https://docs.npmjs.com/getting-started/installing-node](google.com)), luego haga:  
  * git clone [https://github.com/ethereum/browser-solidity](google.com)  
  * cd browser-solidity  

## **DESARROLLO:**

Ejecute npm start y abra [http://127.0.0.1:8080](google.com) en su navegador.
Luego abre tu editor de texto y comienza a desarrollar. El navegador se actualizará automáticamente cuando se guarden los archivos  

## **Resolución de problemas de construcción**  

Aquí hay algunas cosas a considerar si tiene problemas para construir el paquete. 
  * Asegúrese de tener la versión correcta de node, npm y nvm. Puede buscar la versión que se prueba en Travis CI mirando.   
  * En sistemas operativos basados ​​en Debian como Ubuntu 14.04LTS, puede que necesite ejecutar apt-get install build-essential. Después de instalar build.
  
## **Examen de la unidad**
Registre nuevos archivos de prueba unitaria en test / index.js. Las pruebas están escritas usando [cinta](google.com).
Ejecute las pruebas unitarias a través de: prueba npm
Para pruebas locales de explorador sin cabeza ejecute npm run test-browser (Requiere selenio para instalarse - se puede hacer con npm run selenium-install)
Ejecutar pruebas unitarias a través de la prueba npm requiere al menos el nodo v7.0.0  
## **Pruebas del navegador**  
Para ejecutar las pruebas de Selenium a través de Nightwatch, sirve la aplicación a través de un servidor web local:  
run serve # comienza el servidor web en localhost: 8080  
Entonces necesitarás:  
  * Tener un servidor Selenium ejecutándose localmente en el puerto 4444.
      +Ejecutar: npm ejecutar test-browser
  * O bien, instale y ejecute SauceConnect.
      +Ejecutar: sc -u <NOMBRE DE USUARIO> -k <ACCESS_KEY> (ver .travis.yml para conocer los valores)





