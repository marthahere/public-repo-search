# Public Repo Search

A self-contained browser app for searching public GitHub repositories. It uses GitHub's repository search API. The HTML, CSS and JavaScript are all in `index.html`. Loading, error and no-results states each have their own message and style.

## Run it

Open `index.html` in a browser. There is nothing to install and no API key is needed. Searches require an internet connection and are subject to GitHub's unauthenticated rate limit.

Type a search such as `bioinformatics` and press **Search**.

## Try the states

The same links are under the search box.

- **Loading:** open `index.html?demo=loading`. It skips the request and leaves the spinner visible.
- **Error:** open `index.html?demo=error` to show a simulated failure and **Try again** button. You can also search with your browser offline to see a connection error.
- **Empty:** search for `stars:>10000000`, or open `index.html?q=stars%3A%3E10000000`. GitHub accepts the search and returns no repositories, so there is no retry button.
