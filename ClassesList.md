## Cinema Management Classes

### Actor
- Properties:
    - Name (string)
    - BirthDate (DateTime)
    - National
    - Photo (string)
- Methods:
    - GetDetails(): string
    - GetAge(): int

### Movie
- Properties:
    - Title (string)
    - Genre (string)
    - Duration (int)
    - ReleaseDate (DateTime)
    - Director (string)
    - Actors (List<Actor>)
    - Rating (double)
- Methods:
    - GetDetails(): string

# Below classes are not yet ready

### MovieScreening
- Properties:
    - Movie (Movie)
    - Theater (Theater)
    - Date (DateTime)
    - Time (DateTime)
- Methods:
    - GetDetails(): string


### Theater
- Properties:
    - Name (string)
    - Capacity (int)
    - Movies (List<Movie>)
- Methods:
    - AddMovie(movie: Movie)
    - RemoveMovie(movie: Movie)
    - GetMovieSchedule(): List<Movie>

### OnlineTheater
- Properties:
    - Name (string)
    - Movies (List<Movie>)
- Methods:
    - AddMovie(movie: Movie)
    - RemoveMovie(movie: Movie)
    - GetMovieSchedule(): List<Movie>

### Ticket
- Properties:
    - Movie (Movie)
    - Theater (Theater)
    - SeatNumber (string)
    - Price (double)
- Methods:
    - CalculatePrice(): double

### Customer
- Properties:
    - Name (string)
    - Age (int)
    - Tickets (List<Ticket>)
- Methods:
    - BuyTicket(movie: Movie, theater: Theater, seatNumber: string)

### Cinema
- Properties:
    - Name (string)
    - Theaters (List<Theater>)
- Methods:
    - AddTheater(theater: Theater)
    - RemoveTheater(theater: Theater)
    - GetTheaterSchedule(): List<Movie>

### CinemaManager
- Properties:
    - Cinemas (List<Cinema>)
- Methods:
    - AddCinema(cinema: Cinema)
    - RemoveCinema(cinema: Cinema)
    - GetCinemaSchedule(): List<Movie>


 