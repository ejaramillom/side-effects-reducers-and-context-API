# side-effects-reducers-and-context-API
React side effects reducers and context API

the main job of react is: 

- Render UI and react to user input
- Evaluate and render JSX
- Manage state and property of elements and components
- React to user events and input
- reevaluate components upon state and properties changes

# side effects (or simply effects)

Anything else different than this list, is a side effect of using react, for example

- Store data in browser storage
- Send http requests to backend servers
- set and manage timers
- others

we use useEffect hook to avoid infinite loops of rendering and re rendering of components when state changes or a request is done

useEffects(() => {function}, [dependencies])

so, the hook calls a function that is called AFTER every component evaluation IF the specified dependencies change

The dependencies are set to let the effect know when to run its function
