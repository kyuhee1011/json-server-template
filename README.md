# JSON Server Template

## Setup

Before opening the Frontend server, you must fork and clone this repository first and open the JSON server. 

```sh
git clone git@github.com:kyuhee1011/json-server-template.git
cd db
```

Then install the dependencies by running:

```sh
npm install
```
Then open the JSON server by running:
```sh
json-server --watch db.json
```
## Seeding Data

To set up your database, update the `db/seeds.json` file to contain an object
with a key pointing to an array of data, like this:

```json
{
  "desserts": [
    {
      "id": 1,
      "name": "Dalgona (Korean sugar candy)",
      "image": "https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Dalgona.jpg/220px-Dalgona.jpg",
      "description": "Sweet Sugar Candy with fun shape",
      "favorite": false
    },
    {
      "id": 2,
      "name": "Korean Fish Shaped Bread (Bungeoppang)",
      "image": "https://upload.wikimedia.org/wikipedia/commons/thumb/a/ad/Boong_o_bbang.jpg/220px-Boong_o_bbang.jpg",
      "description": "Bungeoppang is a fish-shaped bread with sweetened red bean filling.",
      "favorite": true
    }
  ]
}
```

Then, run `npm run seed` to copy data from the `db/seeds.json` file to the
`db/db.json` file. `json-server` uses the `db.json` file to create your RESTful
API, so make sure your `db.json` file is always up to date!

Any time you want to reset your database back to your original data, run
`npm run seed` again. Doing this will overwrite all the data in your `db.json`
file, so make sure you don't have any data in that file that you don't mind
losing!


### Making Updates

Whenever you made a change, please update your GitHub Repository by running the code below.

```sh
git add .
git commit -m "Updated database"
git push
```

## Frontend code GitHub Repository

https://github.com/kyuhee1011/kyuhee-react-project
