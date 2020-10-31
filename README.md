# tracker-database

In order to patch the database we must run the following command

docker run --rm -v E:\ProyectosDesarrollo\Tracker\tracker-database\liquibase:/liquibase/ -e "LIQUIBASE_URL=jdbc:postgresql://172.17.0.2:5432/tracker" -e "LIQUIBASE_USERNAME=postgres" -e "LIQUIBASE_PASSWORD=password" -e "LIQUIBASE_CHANGELOG=/liquibase/root.xml" webdevops/liquibase:postgres update

You must replace ${route-to-tracker-database} for the route the tracker-database project is located.