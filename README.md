##WDInstagram

### Prompt
Today you're going to make your own version of Instagram (or something very close to it!). Your photo feed app will have full CRUD capability and operate on a single Entry model.

An Entry has the following:

* `author`
* `photo_url`
* `date_taken`

Your app should have the following RESTful actions:

* index (displays all entries)
* show (displays a specific entry)
* new (displays a form to create a new entry)
* create (saves a new entry it to the database)
* edit (displays a form for editing a particular entry)
* update (takes input from the edit form and updates the entry in the db appropriately)
* destroy (deletes a specific entry from the database)

### Instructions

1. Write 5 user stories for your app.
  * Keep it simple and think about what functionality your MVP needs.
2. Create a database: `$ createdb wdinstagram`
3. Create an Entry model
4. Create a `wdinstagram_schema.sql` schema file and generate a table for your Entry model.
  * When ready, migrate your schema into PSQL: `$ psql -d wdinstagram < db/wdinstagram_schema.sql`
5. Create seed data in `$ db/seeds.rb`
  * When ready, run your seeds file: `$ ruby db/seeds.rb`
6. Create routes for your app, mapping them to the RESTful actions listed above
7. Create the views for your routes

### Bonus

1. Add a column for `caption` to your Entry, which is a text description of the shot. You'll need to generate a database migration for this and then update the rest of your app to be able to display these captions.
2. Add "Like" functionality to your posts.
3. Create a route that shows all the posts by a given author.
4. Add a second "Comments" model to your app so that users may leave comments on each of your Entries.
5. Give your Comments model full CRUD capability.
