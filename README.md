# API REST: Calculadora IMC

API que permite gestionar datos y calcular estadísticas relacionadas con el Índice de Masa Corporal (IMC) basado en información del usuario.

## Introducción

La API Calculadora IMC permite:  
- Registrar datos personales y académicos de los usuarios.
- Consultar el IMC promedio por edad, género y programas académicos.
- Acceder a datos básicos de géneros y programas disponibles.

---

## Instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/nicoackerman/api-calculadora-imc

2. Ejecuta el servidor en local:
   ```bash
   npm run dev

## End-Points
### Endpoints

| Método    | Endpoint                                   | Descripción                                                                                         |
|-----------|------------------------------------------- |-----------------------------------------------------------------------------------------------------|
| **POST**  | `/registers`                               | Crea un registro con los datos del usuario.                                                         |
| **GET**   | `/registers/genders`                       | Retorna una lista de géneros disponibles.                                                           |
| **GET**   | `/registers/programs`                      | Retorna una lista de programas académicos válidos.                                                  |
| **GET**   | `/registers/bmi/average/adults`            | Retorna el IMC promedio por edad (a partir de los 19 años).                                         |
| **GET**   | `/registers/bmi/average/genders`           | Retorna el IMC promedio por género.                                                                 |
| **GET**   | `/registers/bmi/average/programs`          | Retorna el IMC promedio por programa académico.                                                     |
| **GET**   | `/registers/genders/id?gender={genero}`    | Retorna el ID del género indicado.                                                                  |
| **GET**   | `/registers/programs/id?program={programa}`| Retorna el ID del programa académico indicado.                                                      |
 
