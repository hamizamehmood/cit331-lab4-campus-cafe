
# Campus Café — Lab 4 Notes

## Task 1: Local HTTP observations

- Local URL: [http://localhost:8080](http://127.0.0.1:5500/index.html)
- Request method: GET
- Status code: 200 OK
- Protocol: HTTP
- What I observed: The browser requested index.html
  from the local development server.



## Bug log (Lab 4, Task 6)

| # | What was wrong (file and line) | Which tool showed it | My fix |
|---|---|---|---|
| 1 | `debug/bugs.html`: stylesheet linked to `style.css`, but file is named `bugs.css` | Network tab | Changed link to `bugs.css` |
| 2 | `debug/bugs.html`: HTML element had no language attribute | Lighthouse / validator | Added `lang="en"` to `<html>` |
| 3 | `debug/bugs.html`: navigation links were inside a generic `div` | Accessibility tree | Replaced `div` with `nav` |
| 4 | `debug/bugs.html`: heading jumped from `h1` to `h4` | Accessibility tree | Changed `h4` to `h2` |
| 5 | `debug/bugs.html`: logo image had no alternative text | Lighthouse | Added descriptive `alt` text |
| 6 | `debug/bugs.html`: label `for` did not match the input `id` | Lighthouse / label click test | Matched both to `email` |
| 7 | `debug/bugs.css`: `colour` is not a valid CSS property | Styles pane | Changed it to `color` |
| 8 | `debug/bugs.css`: missing semicolon after hover background declaration | Styles pane | Added the semicolon |
| 9 | `debug/bugs.css`: `.notes` did not match the HTML class `.note` | Elements / Styles pane | Changed selector to `.note` |
| 10 | `debug/bugs.css`: paragraph text color had insufficient contrast on white | Lighthouse | Changed text color to `#555555` |
