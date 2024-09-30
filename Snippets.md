# React-SnippetsShortcuts
Usefull shortcut snippets for react and javascript.
#Create Context Provider and Hook snippet:
	
    "reactContext": {
	  "prefix": "rc",
	  "scope": "javascript,typescript,javascriptreact",
	  "body": [
		"import { createContext, useContext } from 'react';",
		"",
		"const ${1:${TM_FILENAME_BASE}} = createContext();",
		"",
		"function ${1:${TM_FILENAME_BASE}}Provider({children}) {",
		"",
		"const value = {}",
		"",
		"\treturn (",
		"\t\t<${1:${TM_FILENAME_BASE}}.Provider value={value}>",
		"\t\t\t{children}",
		"\t\t</${1:${TM_FILENAME_BASE}}.Provider>",
		"\t)",
		"}",
		"",
		"function use${1:${TM_FILENAME_BASE}}() {",
		"const context = useContext(${1:${TM_FILENAME_BASE}});",
 		"if (context === undefined)",
   		"throw new Error('Context was used out of the Provider');}",
		"",
		"export {${1:${TM_FILENAME_BASE}}Provider, use${1:${TM_FILENAME_BASE}}}",
  
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
	"reactComponent": {
	  "prefix": "rfc",
	  "scope": "javascript,typescript,javascriptreact",
	  "body": [
		"function ${1:${TM_FILENAME_BASE}}() {",
		"\treturn (",
		"\t\t<div>",
		"\t\t\t$0",
		"\t\t</div>",
		"\t)",
		"}",
		"",
		"export default ${1:${TM_FILENAME_BASE}}",
		""
	  ],
	  "description": "React component"
	},
     	"Print to console": {
	  "prefix": "cl",
	  "scope": "javascript,typescript,javascriptreact",
	  "body": ["console.log($1)"],
	  "description": "console.log"
	},
