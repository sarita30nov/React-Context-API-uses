<p># React-Context-API-uses<br />Below description show how to implement context in React JS</p>
<p>Step1: Create File context.js and write the code</p>
<p><br />import React from 'react';</p>
<p>const ThemeContext = React.createContext();<br />export const ThemeProvider = ThemeContext.Provider;<br />export const ThemeConsumer = ThemeContext.Consumer;</p>
<p>Step 2: pass the value</p>
<p>import { ThemeProvider } from './context';</p>
<p>&lt;ThemeProvider value={{name:'Syntax of ontext'}}&gt;<br />&lt;App/&gt;<br />&lt;/ThemeProvider&gt;<br /><br />Step: 3: consume the value in any child component of &lt;App/&gt;<br /><br />import { ThemeConsumer } from './context';</p>
<p>&lt;ThemeConsumer&gt;<br />{(value)=&gt;&lt;div&gt;{value.name}&lt;/div&gt;}<br />&lt;/ThemeConsumer&gt;</p>
