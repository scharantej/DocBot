## Design for Application that indexes the Whole Godot 4 Documentation

### HTML Files

- *index.html*:
  - Serves as the application's home page.
  - Provides an introduction to the application and its purpose.
  - Includes a search bar for querying the Godot 4 documentation.

- *results.html*:
  - Displays the search results when a user performs a query.
  - Lists the relevant documentation pages with their titles and brief descriptions.
  - Allows users to navigate to the specific pages for more detailed information.

### Routes

- *"/"*:
  - Binds to the root URL ("/") and serves the *index.html* file.
  - Displays the home page of the application and provides an introduction to its functionality.

- *"/search"*
  - Binds to the "/search" URL and handles search queries.
  - Accepts a search term as a query parameter and performs a search against the Godot 4 documentation.
  - Renders the *results.html* file with the search results, displaying the relevant documentation pages and their information.

- *"/docs/<page_name>"*:
  - Binds to the "/docs/<page_name>" URL pattern, where "<page_name>" represents the name of a specific documentation page.
  - Serves the specified documentation page from the Godot 4 documentation.
  - Allows users to navigate to and view the content of individual documentation pages.