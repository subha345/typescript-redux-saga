# React App
 __React__,
 __Redux__,
 __Redux-Saga__,
 __TypeScript__,
 __ESLINT__,
 __Prettier__,
 __Husky__
 
### Git Repo
https://github.com/subha345/typescript-redux-saga

### For Readme styling
https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

# Create initial template
Reference URL: 
https://redux-toolkit.js.org/introduction/getting-started

command: 
npx create-react-app my-app --template redux-typescript

Description: 
1. Include initial store set up with thunk
2. Include typescript hook setup for useAppDispatch and useAppSelector

configureStore():
 wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.
createReducer():
 that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements. In addition, it automatically uses the immer library to let you write simpler immutable updates with normal mutative code, like state.todos[3].completed = true.
createAction():
 generates an action creator function for the given action type string. The function itself has toString() defined, so that it can be used in place of the type constant.
createSlice(): accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.
createAsyncThunk:
 accepts an action type string and a function that returns a promise, and generates a thunk that dispatches pending/fulfilled/rejected action types based on that promise
createEntityAdapter:
 generates a set of reusable reducers and selectors to manage normalized data in the store
 The createSelector utility from the Reselect library, re-exported for ease of use.

# To Read
react-dom/client
Why useAppDispatch and useAppSelector

# REDUX SAGA

is a library that aims to make application side effects (i.e. asynchronous things like data fetching and impure things like accessing the browser cache) easier to manage, more efficient to execute, easy to test, and better at handling failures.
