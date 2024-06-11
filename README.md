# Django Poll App

Django Poll App is a full-featured polling application where users can register to participate in polls. Users can view polls, vote, and see results, while poll owners have additional privileges for managing polls and choices.

## Features

- User Registration and Authentication
- Poll Voting System
  - Users can vote on polls
  - Users cannot vote on the same poll more than once
- Poll Management (for poll owners)
  - Add, edit, update, delete polls
  - Add, update, delete choices
  - End a poll
- View Poll Results
  - Ended polls show final results
- Search and Filter Polls
  - Search polls by name
  - Filter polls by publish date, number of votes
- Pagination
  - Pagination works seamlessly with search and filter options

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/mehakaijaz/poll-app.git
    cd django-poll-app
    ```

2. Create a virtual environment and activate it:

    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the dependencies:

    ```sh
    pip install -r requirements.txt
    ```

4. Apply migrations and create the database:

    ```sh
    python manage.py migrate
    ```

5. Create a superuser to access the admin interface:

    ```sh
    python manage.py createsuperuser
    ```

6. Run the development server:

    ```sh
    python manage.py runserver
    ```

7. Access the app at `http://127.0.0.1:8000/`

## Usage

### User Registration and Login

- Register for an account to participate in polls.
- Log in with your credentials to vote and manage your polls.

### Poll Voting

- View available polls on the homepage.
- Click on a poll to view its details and vote.
- If you have already voted, you cannot vote again.

### Poll Management (For Poll Owners)

- After logging in, access your dashboard to manage polls.
- Create new polls and add choices.
- Edit and update existing polls and choices.
- Delete polls and choices if necessary.
- End a poll to finalize it and show the results to users.

### Search and Filter

- Use the search bar to find polls by name.
- Filter polls by publish date or number of votes using the available options.
- Pagination ensures a smooth browsing experience even with filters applied.

