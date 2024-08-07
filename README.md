<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Ejecutar desarrollo

1. Clonar repositorio
2. Ejecutar
```
yarn install
```
3. Tener Nest CLI instalado
```
npm i -g @nestjs/cli
```

4. Levantar la Base de Datos
```
docker-compose up -d
```

5. Clonar el archivo ___.env.template___ y renombrar a ___.env___

6. llenar las variables de entorno definidas

7. Ejecutar la aplicacion en dev: 

```
yarn start:dev
```

8. Cargar la BD con la semilla ***Unicamente en Desarrollo***
```
http://localhost:3000/api/v2/seed
```


## Stack usado
* MongoDB
* NestJS


## Build de producción 
1.  crear el archivo ```.env.prod```
2. Llenar las variables de entorno productivas
3. Crear la nueva imagen:
```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build  
```
