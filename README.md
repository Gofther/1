# Project Methods
1) POST - https://biletka-sv.ru:8443/Voronezh/event - Создаёт новое мероприятие
   ## Description: Создаёт новое мероприятие по введённым данным
   
    ### Request body - 
    ### {
    ```
    basic_information:{
    name: String,
    name_rus: String,
    event_type: String,
    genre: [String],
    age_rating: Integer,
    organizer: String,
    pushkin: Boolean,
    event_id_culture: Long,
    img_id: Long,
    show_in_poster: Boolean 
    },
   ```
    ```
    duration:{
    hours: Integer,
    minutes: Integer 
    },
    ```
   ```
    additional_information:{
    director: String,
    writer_or_artist: String,
    autor: String,
    actors: [String],
    tags: [String] 
    },
   ```
   ```
    web_widget:{
    signature: String,
    description: String,
    rating_yandex_afisha: Double,
    link: String
   ```
   ### }
   ## }
    
   ## Response body: 
   ## {
    ```
    Id: Long,
    symbolicName: String
   ```
   ## }
   
