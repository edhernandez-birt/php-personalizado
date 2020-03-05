FROM mysql:5.7

# Dejo comentadas las pruebas que he hecho para git clone
#RUN apt-get update \
#	&& apt-get install ssh --yes \
#   	&& apt-get install git --yes  \
#   	&& eval "$(ssh-agent -s)" \
#	&& ssh-keyscan -H github.com >> /etc/ssh/ssh_known_hosts \
#	&& git clone git@github.com:deaw-birt/despliegue-PHP.git /var/www/html \

#	&& git clone https://github.com/deaw-birt/despliegue-PHP.git /var/www/html \
#	&& mv /var/www/html/mysql/InsertarDatos.sql /var/www/html/mysql/insertarDatos.sql 
#	&& cp /var/www/html/mysql/crearBBDD.sql /docker-entrypoint-initdb.d/ \
#	&& cp /var/www/html/mysql/insertarDatos.sql /docker-entrypoint-initdb.d/
	
			
COPY crearBBDD.sql insertarDatos.sql /docker-entrypoint-initdb.d/

EXPOSE 3306