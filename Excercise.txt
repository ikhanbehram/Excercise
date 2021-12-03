                                                      Vacuole

                                       Django framework Assessment Task


   • Develop migrations that creates three tables in MySQL database i.e
     countries, users & posts.

   • Develop relationship such that user belongs to a country while user has
    many posts.
   • Insert dummy data into these tables
   • Develop a Restful API with following requirements:


    Route : POST

  Body : {
    “country” : “XXXXX”,
     “date” : “XXXX-XX-XX”
      }

  Response : {
              id: “XXX”
              name : “XXX”,
             country: “XXX”,
             posts: [
                       {
                         id : “XXX”,
                         title : “XXX”,
                         created_at : “XXXX-XX-XX”
                        },
                        {
                         id : “XXX”,
                         title : “XXX”,
                         created_at : “XXXX-XX-XX”
                         }
                     ]
              }

Description : 
     In a POST request route, the POST request body will take country
     that will be the country of the user and date that will be the date when a post was
     created by a user. Using these two filters data the API will filter the response and
     return something like the above example response that contains user id, user
     name, country name, and the users many posts with post id and post title and
     post created_at which will be the date on which the post was created by the user.
     The response will be filtered in such a way that only those users data will be
     returned that has a specific country matching with the country coming in the
     POST request body and the user has one or more posts created on the date which
     was specified in the POST request body.