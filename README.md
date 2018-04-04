## RSS Feeds
1. check if there are variable, allFeeds
2. check if there are no empty
3. check if all properties of each object of allFeeds are defined and not empty by for loop to loop all objects

## The menu
1. If the menu is hidden, 'body' tag has class 'menu-hidden'. Therefore, the test is to check if the 'body' tag has this class, if yes, the menu is hidden by default.
2. By JQuery, .click() can trigger the click event and check if the menu icon is working by clicking it

## Initial Entries
1. Since loadFeed() is asynchronous, we need to use beforeEach and done().
2. By using done(), we can check if loadFeed() is completely loaded and also the content and structure are defined and not empty.

## New Feed Selection
1. Since loadFeed() is asynchronous, we need to use beforeEach and done().
2. By running loadFeed() with id = 0, the header and headline can be obtained. Then we can run loadFeed(1) to compare if the content of both are changed.
3. Lastly, run loadFeed(0) again to return to default in order to let user to use the app after testing.
