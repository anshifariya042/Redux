 const { createStore } = require('redux');

const initialState={
    count:0
};

function counter(state=initialState,action){
    switch(action.type){
        case 'INCREMENT':
            return {count:state.count+1};
        case 'DECREMENT':
            return {count:state.count-1};
        default:
            return state;     
    }
}
const store = createStore(counter);
 store.subscribe(() => {
  console.log('Current state:', store.getState());
});
store.dispatch({ type: 'INCREMENT' }); 
store.dispatch({ type: 'INCREMENT' }); 
store.dispatch({ type: 'DECREMENT' }); 
