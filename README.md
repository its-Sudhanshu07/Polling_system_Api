# Polling System API

A Polling System API using NOde JS and MongoDB have Multiple Features

# Features:

1. Create a question.
2. Add options to a question.
3. Add a vote to an option of a question.
4. Delete a question (only if none of its options have votes).
5. Delete an option (only if it has no votes).
6. View a question with its options.


# Routes:

POST /questions/create  Create a new question.
Key: question,
Value: "Your Question"

POST /questions/:id/options/create  Add options to a specific question.
Key: option,
Value: "Your Option"

GET /questions/:id/delete    Delete a question (if no votes are associated with any option).

GET /options/:id/delete   To Delete an option (if it has no votes).

POST /options/:id/add_vote: Increment the vote count for a specific option.

GET /questions/:id   View a question and its options, including the votes given to each option.

# Folder Structure:
├── config
│ --- └── mongoose.js
├── controllers
│ --- └──optionsController.js
│ --- └──questionsController.js
├── models
│ --- ├── Options.js
│ --- └── Questions.js
├── routes
│ --- ├── api
│          ├── v1
                ├── index.js
                ├── option.js
                ├── question.js
            ├── index.js
│ --- ├── index.js
├── .gitignore
├── package.json
├── package-lock.json
├── README.md
└── index.js
# Hosted Link:(https://polling-system-api-3gvy.onrender.com )



