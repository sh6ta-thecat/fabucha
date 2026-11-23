FABUCHA - ESTRUCTURA INICIAL
============================

Este ZIP contiene las carpetas y archivos base del proyecto. Las páginas y
clases son esqueletos iniciales: no representan todavía un sistema funcional.

REQUISITOS
----------
- PHP 8.1 o superior
- Composer
- MySQL o MariaDB
- Apache con mod_rewrite y AllowOverride habilitados

INSTALACIÓN DE DEPENDENCIAS
---------------------------
1. Extrae la carpeta fabucha dentro de htdocs.
2. Abre una terminal dentro de la carpeta del proyecto.
3. Ejecuta: composer install
   Composer generará composer.lock y la carpeta vendor/.
4. Crea la base de datos indicada en config.php.
5. Ajusta las credenciales y APP_URL en config.php.
6. Abre http://localhost/fabucha/public/

IMPORTANTE
----------
- vendor/ y composer.lock no se incluyen porque deben ser generados por Composer.
- No guardes archivos sensibles ni credenciales en public/.
- uploads/.htaccess bloquea el acceso directo a los archivos subidos.
- Antes de producción, configura APP_ENV como production y revisa permisos,
  validaciones, autenticación, autorización y protección CSRF.
