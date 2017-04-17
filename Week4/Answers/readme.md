Answer 4.1: 
    - The number od milestones for a company rarely exceeds 10 per year.
    - One frequently displayed vie of our data displays company details such as the "name", "founded_year", "twitter_username", etc. as well as milestones. 

Answer 4.2: 
    - B

    db.categories.insertOne({"_id": "Quantum Mechanics", "ancestors": ["Books", "Science", "Physics"], "parent": "Physics"})
    db.categories.insertOne({"_id": "Classical Mechanics", "ancestors": ["Books", "Science", "Physics"], "parent": "Physics"})
    db.categories.insertOne({"_id": "Physics", "ancestors": ["Books", "Science"], "parent": "Science"})
    db.categories.insertOne({"_id": "Chemistry", "ancestors": ["Books", "Science"], "parent": "Science"})
    db.categories.insertOne({"_id": "Science", "ancestors": ["Books"], "parent": "Books"})
    db.categories.insertOne({"_id": "Books", "ancestors": [], "parent": null})

Answer 4.3:
    - Can make atomic updated as books are checked out or turned in.

