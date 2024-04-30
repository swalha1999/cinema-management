## Cinema Management Classes

### Person
- Properties:
    - Name (string)
    - BirthDate (DateTime)
    - National
    - Photo (string) // URL of the photo optional
- Methods:
    - GetDetails(): string
    - GetAge(): int

### Actor : Person
- Properties:
    - Movies (List<Movie>)
- Methods:
    - GetMovies(): List<Movie>

### Director : Person
- Properties:
    - Movies (List<Movie>)
- Methods:
    - GetMovies(): List<Movie>

### Genre
- Properties:
    - Name (string)
    - Description (string)
- Methods:
    - GetDetails(): string
    - GetName(): string
    - GetDescription(): string

### Movie
- Properties:
    - Title (string)
    - Genre (Genre)
    - Duration (int)
    - ReleaseDate (DateTime)
    - Director (Director)
    - Actors (List<Actor>)
    - Rating (double)
- Methods:
    - GetDetails(): string
    - GetActors(): List<Actor>
    - GetDirector(): Director
    - GetGenre(): Genre
    - GetRating(): double
    - GetReleaseDate(): DateTime
    - GetDuration(): int
    - AddActor(actor: Actor)
    - RemoveActor(actor: Actor)
    - SetDirector(director: Director)
    - SetGenre(genre: Genre)
    - SetRating(rating: double)
    - SetReleaseDate(releaseDate: DateTime)
    - SetDuration(duration: int)
    - AddRating(rating: double)



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


 