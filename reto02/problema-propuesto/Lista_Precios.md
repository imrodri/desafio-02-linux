confidencial


# 4. Problema propuesto
   
Roxs es la líder de un equipo de trabajo para una compañía que realiza Auditorías Externas. Él ha creado un archivo llamado *Lista_Precios* en su directorio `/home`. El archivo es altamente confidencial, pero resulta que existe un alto riesgo de que su archivo  sea  vulnerado  porque  otros  empleados  utilizan  su  equipo  al  finalizar  su turno.   Actualmente,   Roxs   posee   una   contraseña   segura,   pero   él   necesita resguardar los datos de ese archivo y no desea que nadie más que solamente él tenga acceso al mismo. ¿Qué solución le propondrían como equipo a Roxs? 

>**Considere lo siguiente para solucionar el problema.** 
>
>Para  proveer  una  solución  apropiada  para  restringir  accesos  no autorizados  al archivo, se necesita realizar lo siguiente: 
>
>1. Identificar las medidas de seguridad a implementarse. 
>2. Identificar el tipo de usuarios para quienes los permisos >serán cambiados. 
>3. Identificar el tipo de permiso que necesita ser cambiado.
>4. Verificar los permisos de acceso al archivo.

### Solucion

1. Medidas de seguridad
- Crear un usuarios para cada usuario que se conecte al dispositivo
- Mover el archivo importante que se encuentre dentro de  `/home`
- Modificar los permisos de lectura y escritura del archivo al usuario o usuarios que pertenezcan al grupo que si puede leer esa informacion

2. Tipos de usuarios

- Usuarios de grupo de auditoria y grupo de usuarios normales
- Dandoles permisos  diferenciados

3. Tipos de permiso a ser cambiados

- Usuarios normales:  chmod o-rwx usuario/home/Lista_Precios 
- Usuarios auditores:  chmod ugo+rwx usuario_audit/home/Lista_Precios 

4. Verificacion de permisos

Podriamos usar el comando `ls -l` para identificar los permisas dados