# proceso-participativo Logo de InnovAnda
Este es el repositorio de código abierto del sitio web de eParticipation CONSUL, desarrollado originalmente para el sitio web de eParticipation del Ayuntamiento de Madrid.
Documentación
Consulte la documentación en curso en https://docs.consulproject.org para obtener más información sobre cómo iniciar su propia bifurcación CONSUL, instalarla, personalizarla y aprender a usarla desde una perspectiva de administrador / mantenedor.

Sitio web principal del Proyecto CONSUL
Puede acceder al sitio web principal del proyecto en http://consulproject.org donde puede encontrar documentación sobre el uso de la plataforma, videos y enlaces al espacio comunitario.

Configuración para entornos de desarrollo y prueba
NOTA : Para obtener instrucciones más detalladas, consulte los documentos

Requisitos previos: instalar git, Ruby 2.5.8, bundlergem, Node.js y PostgreSQL (> = 9.4).

clon de git https://github.com/consul/consul.git
 cd cónsul
instalación del paquete
cp config / database.yml.example config / database.yml
cp config / secrets.yml.example config / secrets.yml
bin / rake db: crear
bin / rake db: migrar
bin / rake db: dev_seed
RAILS_ENV = test rake db: configuración
Ejecute la aplicación localmente:

contenedor / rieles s
Ejecute las pruebas con:

bin / rspec
Puede utilizar el usuario administrador predeterminado del archivo de semillas:

usuario: admin@consul.dev contraseña : 12345678

Pero para algunas acciones como votar, necesitará un usuario verificado, el archivo de semillas también incluye uno:

usuario: verificado@consul.dev contraseña: 12345678

Configuración para entornos de producción
Ver instalador

Estado actual
El desarrollo comenzó el 15 de julio de 2015 . Code se implementó en producción el 7 de septiembre de 2015 para decide.madrid.es . Desde entonces, a menudo se agregan nuevas funciones. Puede echar un vistazo a las funciones actuales en el sitio web del proyecto y las funciones futuras en la Hoja de ruta y la lista de problemas abiertos .

Licencia
Código publicado bajo AFFERO GPL v3 (ver LICENCIA-AGPLv3.txt )

Contribuciones
Ver CONTRIBUTING.md
