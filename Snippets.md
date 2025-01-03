# React-SnippetsShortcuts
Usefull shortcut snippets for react and javascript.
#Create Context Provider and Hook snippet:
	
    {
	"Print to console": {
	  "prefix": "cl",
	  "scope": "javascript,typescript,javascriptreact",
	  "body": ["console.log($1)"],
	  "description": "console.log"
	},
	"reactComponent": {
	  "prefix": "rfc",
	  "scope": "javascript,typescript,javascriptreact",
	  "body": [
		"export default function ${1:${TM_FILENAME_BASE}}() {",
		"\treturn (",
		"\t\t<div>",
		"\t\t\t$0",
		"\t\t</div>",
		"\t)",
		"}",
		"",
		""
	  ],
	  "description": "React component"
	},
	"reactContext": {
	  "prefix": "rc",
	  "scope": "javascript,typescript,javascriptreact",
	  "body": [
		"import { createContext, useContext } from 'react';",
		"",
		"const Context = createContext();",
		"",
		"function ${1:${TM_FILENAME_BASE}}Provider({children}) {",
		"",
		"const value = {}",
		"",
		"\treturn (",
		"\t\t<Context.Provider value={value}>",
		"\t\t\t{children}",
		"\t\t</Context.Provider>",
		"\t)",
		"}",
		"",
		"function use${1:${TM_FILENAME_BASE}}() {",
		"const context = useContext(Context);",
 		"if (context === undefined)",
   		"throw new Error('Context was used out of the Provider');",
		"return context}",
		"",
		"export {${1:${TM_FILENAME_BASE}}Provider, use${1:${TM_FILENAME_BASE}}}"

	  ],
	  "description": "React Context Template"
	},
	"useEffect Template": {
	  "prefix": "ue",
	  "scope": "javascript,typescript,javascriptreact",
	  "body": [
		"useEffect(()=>{},[])"
	  ],
	  "description": "React component"
	},
	"useState Template": {
	  "prefix": "us",
	  "scope": "javascript,typescript,javascriptreact",
	  "body": [
		"const [state,setState] = useState();"
	  ],
	  "description": "React component"
	},
	"useRef Template": {
	  "prefix": "ur",
	  "scope": "javascript,typescript,javascriptreact",
	  "body": [
		"const ref = useRef();"
	  ],
	  "description": "React component"
	},
	"reactStyledComponent": {
	  "prefix": "rsc",
	  "scope": "javascript,typescript,javascriptreact",
	  "body": [
		"import styled from 'styled-components'",
		"",
		"const Styled${TM_FILENAME_BASE} = styled.$0``",
		"",
		"function ${TM_FILENAME_BASE}() {",
		"\treturn (",
		"\t\t<Styled${TM_FILENAME_BASE}>",
		"\t\t\t${TM_FILENAME_BASE}",
		"\t\t</Styled${TM_FILENAME_BASE}>",
		"\t)",
		"}",
		"",
		"export default ${TM_FILENAME_BASE}",
		""
	  ],
	  "description": "React styled component"
	},
	"importCSSModule": {
    "prefix": "csm",
    "scope": "javascript,typescript,javascriptreact",
    "body": ["import styles from './${TM_FILENAME_BASE}.module.css'"],
    "description": "Import CSS Module as `styles`"
	  },
	  }
  
