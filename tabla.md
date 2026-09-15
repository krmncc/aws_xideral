# 1.- Crear tabla peliculas_carmen
  
    CREATE TABLE `cine`.`peliculas_nombre` (
    `pelicula_id` INT NOT NULL AUTO_INCREMENT,
    `nombre` VARCHAR(45) NOT NULL,
    `director` VARCHAR(45) NOT NULL,
    `genero` VARCHAR(45) NOT NULL,
    `anio_estreno` VARCHAR(45) NOT NULL,
    `duracion_minutos` VARCHAR(45) NOT NULL,
    `calificacion` VARCHAR(45) NOT NULL,
    `disponible` VARCHAR(45) NULL,
    PRIMARY KEY (`pelicula_id`));
## LLenar tabla
    INSERT INTO `cine`.`peliculas_nombre` (`pelicula_id`, `nombre`, `director`, `genero`, `anio_estreno`, `duracion_minutos`, `calificacion`, `disponible`) VALUES ('1', 'iron man 1', 'Jon Favreau', 'Accion/Ciencia ficcion', '2008', '126', '7.9', 'Disney+');
    INSERT INTO `cine`.`peliculas_nombre` (`pelicula_id`, `nombre`, `director`, `genero`, `anio_estreno`, `duracion_minutos`, `calificacion`, `disponible`) VALUES ('2', 'iron man 2', 'Jon Favreau', 'Accion/Ciencia ficcion', '2010', '124', '6.9', 'Disney+');
    INSERT INTO `cine`.`peliculas_nombre` (`pelicula_id`, `nombre`, `director`, `genero`, `anio_estreno`, `duracion_minutos`, `calificacion`, `disponible`) VALUES ('3', 'iron man 3', 'Shane Black', 'Accion/Ciencia ficcion', '2013', '130', '7.1', 'Disney+');
    INSERT INTO `cine`.`peliculas_nombre` (`pelicula_id`, `nombre`, `director`, `genero`, `anio_estreno`, `duracion_minutos`, `calificacion`, `disponible`) VALUES ('4', 'intensamente 1', 'pete docter', 'Imaginatiba', '2015', '90', '9.0', 'Amazon');
    INSERT INTO `cine`.`peliculas_nombre` (`pelicula_id`, `nombre`, `director`, `genero`, `anio_estreno`, `duracion_minutos`, `calificacion`, `disponible`) VALUES ('5', 'intensamente 2', 'pete docter', 'Infantil', '2025', '156', '8.6', 'Disney+');
    INSERT INTO `cine`.`peliculas_nombre` (`pelicula_id`, `nombre`, `director`, `genero`, `anio_estreno`, `duracion_minutos`, `calificacion`, `disponible`) VALUES ('6', 'red', 'Domee Shi', 'Infantil', '2022', '160', '6.9', 'Disney+');
    INSERT INTO `cine`.`peliculas_nombre` (`pelicula_id`, `nombre`, `director`, `genero`, `anio_estreno`, `duracion_minutos`, `calificacion`, `disponible`) VALUES ('7', 'wolverine', 'na', 'superheroe', '2009', '135', '7.8', 'Netflix');
    INSERT INTO `cine`.`peliculas_nombre` (`pelicula_id`, `nombre`, `director`, `genero`, `anio_estreno`, `duracion_minutos`, `calificacion`, `disponible`) VALUES ('8', 'Wolverine: Inmortal', 'na', 'superheroe', '2013', '157', '8.3', 'Netflix');
    INSERT INTO `cine`.`peliculas_nombre` (`pelicula_id`, `nombre`, `director`, `genero`, `anio_estreno`, `duracion_minutos`, `calificacion`, `disponible`) VALUES ('9', 'Logan', 'na', 'superheroe', '2017', '170', '9.5', 'Netflix');
    INSERT INTO `cine`.`peliculas_nombre` (`pelicula_id`, `nombre`, `director`, `genero`, `anio_estreno`, `duracion_minutos`, `calificacion`, `disponible`) VALUES ('10', 'spiderman 1', 'na', 'superheroe', '2001', '187', '8.3', 'Netflix');

### Mostrar todas las películas.
    SELECT * FROM cine.peliculas_nombre;

### Mostrar solamente el título, género y año de estreno.


