# MVP #
    The app should be able to perform CRUD operations on multiple models (Song, Album, Artist, etc) as well as have routes to display information as JSON. The app should also include all migrations for database models.

# MoSCoW #
    Must have:
        As part of your pseudocode, you will need to create and submit for approval an object relationship diagram using diagrams.net or dbdiagram.io before you get started with your project in code.

        The db diagram should take into consideration and show:
        Relationships between different tables
        Considerations for null, blank fields and default values or other “options”
        Note: In Django you don’t have to create ManyToMany tables for relationships but in your diagram you will need to account for those. 
        Create models in Django to store data in a PostgreSQL database. The basic requirements are to have at least one (1) foreign key relationships and one (1) many to many relationships to correctly link data.

        Show READ functionality of all models through url collections from DRF with Thunder Client (VSCode Extension) requests for all models to get all data in each table/model.

        Implement full CRUD operations for, at the very least, one model with at least one relationship.
        
        Use Django Rest Framework to build an api and routes for queries.
        
        Use Thunder Client to prove the functionality of the Create, Read, Update, and Delete Routes. You can also test some routes in the browser, as long as they are GET routes.
        
#### Route Requirements: ####
    
        GET for all models at /api/[model-name]/ - returns all objects for that model (nested data is unnecessary for MVP, just FKs in the field data is ok)
        
        GET for single instances of models /api/[model-name]/[pk]/ - returns a single object
        
        POST routes for each model at /api/model-name
        
        UPDATE routes for each model at /api/model-name/pk
        
        DELETE routes for each model at /api/model-name/pk

    Should have:
        Build a route to allow a user to add a song to a playlist
        Build routes that accept query parameters (?query=search) to search/filter for some data or all models. DRF Documentation 
        
    Could have:
        Create a route that filters a list of songs by artist or some other functionality.
        Add a custom field(s) to the API that keeps track of the most popular songs based on playlists additions.

    Won't have:
        Hook this DB up to a React frontend. 
        
# Data flow diagram #

![Music flow diagram](img/django%20jams.png)