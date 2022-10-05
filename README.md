# Instructions

1. Build and run the server

``` bash
git checkout react-17 # or react-18
npm install
npm run build
node build/server.js
```

2. Open `localhost:3000` in Chrome. Open the Chrome DevTools, go to the Network tab, and set the speed to "Slow 3G".

3. Refresh the page. Before the JS finishes downloading, try typing in the text box.

4. Once hydration completes, you'll see the "value is: " text still showing an empty string. Thus the DOM content of the input box is out of sync with the React state. If another React state update happens, the box content will be blown away.
