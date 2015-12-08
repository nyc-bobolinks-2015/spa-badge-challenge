## SPABadge

Mr. Merriwether is opening up a competitor bootcamp and wants to hire DBC students to make another version of BootBadge.

Here's the BootBadge app: http://bootbadge.herokuapp.com/cohorts/63

TodoMVC has helpful tips for features you may need: https://github.com/tastejs/todomvc/tree/gh-pages/examples/vanillajs

For a given cohort, each student has a page that contains "badges" with a given catchphrase.
Visitors to the site can vote for their favorite badge on each student's page. The badges should appear from most popular at the top to least popular at the bottom.

Mr. Merriwether read a Medium post that said JavaScript applications are the future and anyone still using a full-stack Rails is an idiot (obviously false).

Because he is the client and funding the project, you need to use JavaScript to make a single-page app version of BootBadge called SPABadge. SPABadge is a "bake-off" to see who should get the contract. The first version will have a single cohort: DBC teachers and mentors.

You can find the main page at spa-badge.html. Click the Sample Page link to see what a teacher's badge page should look like.

Rules
- Has to be a JavaScript app that utilizes your miniQuery library
- Uses MVC architecture. See TodoMVC for inspiration: https://github.com/tastejs/todomvc/tree/gh-pages/examples/vanillajs
- Only XHR / ajax requests to the server are allowed except for the initial app load
- Use vanilla javascript rather than jQuery - you can use your miniQuery to help
- Don't use frameworks such as Angular
- All page navigation must be done through client-side JS routing (see Considerations section)
- Data should be persisted on a Rails API backend. Your Rails app should not serve / have any erb or haml files. You should design an appropriate API.
- All DOM manipulation should take place on the client

Considerations
- Badge sorting by vote count.
- Routing. http://myapp.com/#/walker should show me Walker's page for example. See the pushState API for implementation ideas: https://developer.mozilla.org/en-US/docs/Web/API/History_API
- Keeping track of votes. Use a cookie to manage how many times a person has voted.
- Security. Escape the user's input to avoid XSS attacks
