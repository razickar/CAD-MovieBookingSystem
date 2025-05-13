# CAD-MovieBookingSystem
Project :- Theatre Movie Booking System.

Title:-  BookNow-Seat.

Type :- B2C

Target audience :- [movie lovers, celebrity Based Fans,Time passers, Family movies audience]

Budget :- currently time is budget.

Members :- 1.

Features:-
 - choosing theatre
 -selecting seat and booking
 - movie recommendations
 -updates
 -Trailers, teasers, shorts or scenes
 -Watchlists 
 -User reviews and ratings
 -Social sharing or comments
 -login page
 -Registration page
 -If user book seat ,then other booking website to show this seat is booked Another booking website to show that if the user books a seat, that seat has already been reserved by users.


Feasibility :-

	- registeration
	-login
	-movie recommendation
	-watchlist
	-choosing theatre
	-(booked seat information)
	-slecting seat ui and booking process
	- sharing or comment
	- review and rating theatre

## DATA MODEL
 Registration class:

	Username: String
	Password: String
	Email: String
	FullName: String
	PhoneNumber: String
	DateOfBirth: Date

Login class:

	Username: String
	Password: String

MovieRecommendation class:

	MovieId: Integer
	Title: String
	Genre: String
	Rating: Float
	ReleaseDate: Date
	IsPopular: Boolean
	ImageUrl: String

Watchlist class:

	WatchlistId: Integer
	UserId: Integer
	MovieId: Integer
	DateAdded: Date

Theatre class:

	TheatreId: Integer
	Name: String
	Location: String
	TotalScreens: Integer
	Rating: Float
	Amenities: List<String>

BookedSeatInformation class:

	BookingId: Integer
	UserId: Integer
	MovieId: Integer
	TheatreId: Integer
	ShowDate: Date
	ShowTime: String
	SeatNumbers: List<String>
	TotalAmount: Float

SeatSelection class:

	ScreenId: Integer
	AvailableSeats: List<String>
	BookedSeats: List<String>
	SeatPrice: Map<String, Float>
	SeatTypes: Map<String, String>
	MaxSeatsPerBooking: Integer

BookingProcess class:

	BookingId: Integer
	UserId: Integer
	MovieId: Integer
	TheatreId: Integer
	ShowDate: Date
	ShowTime: String
	SelectedSeats: List<String>
	PaymentMethod: String
	BookingStatus: String
	TotalAmount: Float

Sharing class:

	SharingId: Integer
	UserId: Integer
	BookingId: Integer
	SharedWith: List<String>
	Message: String
	SharingDate: Date

Comment class:

	CommentId: Integer
	UserId: Integer
	MovieId: Integer
	Content: String
	CommentDate: Date
	Likes: Integer

Review class:

	ReviewId: Integer
	UserId: Integer
	TheatreId: Integer
	Rating: Integer
	Comment: String
	ReviewDate: Date
	Helpful: Integer
