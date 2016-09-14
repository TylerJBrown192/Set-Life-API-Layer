# Set Life (API Layer)

This is the repository for the Rails 5 API Layer of the Set Life application, eventually located at [SetLife.live](#).

Set Life is an application for users who love all things music - concerts, bands, albums, reviews, everything.

Eventually this README will detail the technologies used for the back end of the application as well as the features it showcases.

You can find the Ember.js UI layer of Set Life [in this repository](https://github.com/TylerJBrown192/Set-Life-UI-Layer).

---------------------------------------------------

### Planned Schema Visualization

![Set Life Schema](https://github.com/TylerJBrown192/Set-Life-API-Layer/blob/master/schema.png "The Initial Schema for the Set Life application")

# Updates

* The UsersSubmittedShows associative table should be changed to a one-to-one relationship, with the Shows table simply pointing towards a UserID.

* Show ratings should be extracted out to the UserAttendedShows associative table and averaged as a whole (possibly change table name to 'Attendees' and change further naming conventions to be more real-world applicable rather than descriptive of the two tables which make up the associative relationship (thanks Brian!))

* Users should be able to rate on a per-Band-per-Show basis as well. This would likely require an associative table between Bands and the UserAttendedShows associative table.

* Bands can join or leave a Tour at any time, thus a BandsShows associative relationship will need to be created (but keep the BandsTours table)

* Decide whether or not to extrapolate a Band's per-Show rating to build out their individual BandRating. Not a huge fan of this idea though, as many Bands can be either much better or worse live than their recorded representation. This idea would likely require a separate associative table for UsersBandRatings

---------------------------------------------------

#### Things that will eventually be covered:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions
