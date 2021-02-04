# database name : Games Library
# list name : Videogames

- id BIGINT PRIMARYKEY NOTNULL AUTO_INCREMENT
- isbn string VARCHAR(10) NOTNULL UNIQUE
- title string TEXT(1000) NOTNULL
- description string TEXT NULL
- software_house string VARCHAR(50) NOTNULL
- engine string VARCHAR(50) NOTNULL
- publisher string VARCHAR(50) NOTNULL
- creators string VARCHAR(100) NULL
- genre string VARCHAR(15) NOTNULL
- price int FLOAT (3,2) 999,99 NULL
- first_release date YEAR NOTNULL
- last_release date YEAR NOTNULL
- availability int TINYINT NULL DEFAULT(1)
- cover_img string VARCHAR() NULL
- language string VARCHAR(20) NOTNULL
- quantity int SMALLINT NULL DEFAULT(0)
- dimension_size int INT NULL
