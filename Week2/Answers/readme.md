Answer 2.1: 
    db.movieDetails.find({$and:[{"year":2013},{"rated":"PG-13"},{"awards.wins":{$eq:0}}]}).pretty()

    - A Decade of Decadence, Pt. 2: Legacy of Dreams

Answer 2.2: 
    db.movieDetails.find({},{tittle:1, _id:0})
    db.movieDetails.find({year:1964},{title:1,_id:0})

Answer 2.3:
    db.movieDetails.find({"countries.1":"Sweden"}).count()
    - 6

Answer 2.4:
    db.movieDetails.find({"genres":["Comedy","Crime"]}).count()
    - 20

Answer 2.5:
    db.movieDetails.find({"genres":{$all:["Comedy","Crime"]}}).count()
    - 56

Answer 2.6:
    - $set