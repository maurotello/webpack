- Ejemplos:  Truffle Box Webpack

  Webpack es un empaquetador de módulos, es decir, te permite generar un archivo único con todos aquellos módulos que necesita tu aplicación para funcionar. Para darte una idea, te permite incluir todos tus archivos javascript .js en un único archivo, incluso se pueden incluir hasta archivos de estilos .css en el mismo archivo, llamado *.bundle.js. Además se puede realizar otras tareas de optimización de los códigos, tales como la minificación y la compresión.

  Utilizaremos este ejemplo que se provee de forma completa utilizando el framework webpack
  Para descargar la solución debemos correr en una carpeta vacía el comando 
    $ truffle unbox webpack

	Modificamos truffle-config.js 
    configuramos Ganache GUI y compilador solc 0.8.3
	Compilamos y migramos contrato a la red ganache
    $ truffle compile
	  $ truffle console --network ganache	
		migrate --reset

- Ejecutamos la dApp
  en otro consola, no donde esta corriendo truffle console
  $ cd app
  $ npm run dev

- Para compilar la aplicación para producción, use el script de build en la carpeta de la app. El build para producción estará en la carpeta app/dist
  $ cd app
  $ npm run build
  