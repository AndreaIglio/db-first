<!-- Istruzioni:
Provare a strutturare il seguente database che modellizza un hotel: Ci sono varie stanze, ognuna con le proprie caratteristiche. Le diverse stanze vengono prenotate per periodi di tempo, da ospiti. Ad ogni prenotazione devono essere associati tutti gli ospiti della stanza.
Nella repo mettete sia il file del diagramma che il file esportato come immagine.
Buon lavoro e buon weekend! -->


# database name : Hotel
# list name : Hotel booking

<!-- Hotel details -->
- hotel_id BIGINT PRIMARYKEY NOTNULL UNIQUE
- name string VARCHAR(20) NOTNULL
- zip_code int TINYINT NOTNULL
- city string VARCHAR(10) NOTNULL
- state string VARCHAR(10) NOTNULL
- phone_number int TINYINT NOTNULL
- rooms int SMALLINT NOTNULL
<!-- Rooms details -->
- room_number SMALLINT PRIMARYKEY NOTNULL
- room_type VARCHAR(20) NOTNULL
- room_status TINYINT NOTNULL
- price TINYINT NOTNULL
- room_beds int TINYINT NOTNULL
- wi-fi string VARCHAR (5) NULL
- tv string VARCHAR(5) NULL
- guest_id BIGINT FOREIGNKEY NOTNULL UNIQUE
<!-- Guest details -->
- guest_id BIGINT PRIMARYKEY NOTNULL UNIQUE
- guest_name VARCHAR (20) NOTNULL
- guest_lastname VARCHAR (20) NOTNULL
- guest_age TINYINT NOTNULL
- guest_phone_number TINYINT NOTNULL
- guest_email VARCHAR(50) NULL
- guest_city VARCHAR(20) NOTNULL
- guest_state VARCHAR (20) NOTNULL
- guest_zip_code TINYINT NOTNULL
<!-- Reservation details -->
- reservation_number BIGINT PRIMARYKEY NOTNULL UNIQUE
- check_in_date DATETIME NOTNULL
- check_out_date DATETIME NOTNULL
- status VARCHAR(20) NOTNULL
- number_of_guests TINYINT NOTNULL
- reservation_date DATETIME NOTNULL


