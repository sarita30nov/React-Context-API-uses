# React-Context-API-uses
Below description show how to implement context in React JS

Step1: Create File context.js and write the code


import React from 'react';

const ThemeContext = React.createContext();
export const ThemeProvider = ThemeContext.Provider;
export const ThemeConsumer = ThemeContext.Consumer;

Step 2: pass the value 

import { ThemeProvider } from './context';

  <ThemeProvider value={{name:'Syntax of  ontext'}}>
  <App/>
  </ThemeProvider>
  
 Step: 3:  consume the value in any child component of  <App/>
 
 import { ThemeConsumer } from './context';

<ThemeConsumer>
{(value)=><div>{value.name}</div>}
</ThemeConsumer>
