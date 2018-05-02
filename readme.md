Inspiration:
    - Game of Life offsite. How to best manage the UI

History:
    - Jquery, the defacto tool for the web that abstracted all the work making things in browsers.
    - More and more stuff using browsers AND THEREFORE, needs better way to manage a complex app and complex state. Just look at the privacy settings page. It is simple and probably the limitation of control.
        - New frameworks to handle this stuff: Angularjs, Backbonejs, etc kickstarted an entire ecosystem to manage complexy. And... kinda added to its complexity...
    - React was a response to the insanity of all of these frameworks. And does some interesting things. It combines javascript+HTML w/ JSX (WTF). Show example. Using a virtual DOM (?)... but the question is why? This talk attempts to answer this question.
    - HEAVILY and ENTIRELY inspired/lifted from: https://www.youtube.com/watch?v=pTHCwUdGFkc. Most content comes from these guys.

Part 1:
    - Code html, CSS // http://colours.neilorangepeel.com/category/green/
    - Has to run through the DOM a lot.

Reflection:
    - How would we be able to save the state and come back?
        - How would we get the turn? or places? We'd have to crawl through the dom and get those things.
    - How would we validate? We'd have to go into the DOM.
    - What if we clicked outside?
    - Writing to the DOM directly is DANGEROUS. Hence, in react there is a method called DANGEROUSLY SET INNER HTML.

Alternative:
    - Let's write to a javascript object and keep all the state there.
    - Then render the whole UI as a representation of that object. If it isn't defined in render function, it can't show up on screen.

Part 2:
    - Create game state object
    - Create render function that takes the state of the game.
    - Refresh with different game states

Reflection:
    - Computationally expensive
    - Stuff that only exists in the client side: Input example
    - JSX potential

Solution:
    - ReactJS

Close:
    - Conway's game of life example