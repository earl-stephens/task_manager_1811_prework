

    Define CRUD.

    Create
    Read
    Update
    Delete

    Operations that can be performed on a resource (which is usually something in the application like tasks, people, movies, etc.).  Each row in a table usually holds a specific instance of a particular resource.

    Why do we use set method_override: true?

    In the form we have set method="post", but we really need it to be PUT.  Setting method_override to true allows us to use a hidden method for PUT, while still conforming to the HTML conventions of forms only allowing GET or POST.

    Explain the difference between value and name in this line: <input type='text' name='task[title]' value="<%= @task.title %>"/>.

    We are setting up our params hash, with name as a key, and value as a value.

    What are params? Where do they come from?

    Params come from the input to a form.  When the user inputs data in the tasks form, they are placed in a params hash.

    Check out your routes. Why do we need two routes each for creating a new Task and editing an existing Task?

    We need this because there needs to be a route to display a form (for user input to create or choose the task to edit), and then there needs to be a route that displays the results of the user's actions.
