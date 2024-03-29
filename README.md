# asd-gobling

## Run locally

Ubuntu Linux
```
cd app
``` 
```
yarn
``` 
```
yarn run dev
```


You need to perform following steps to run project locally.
```
cd app
``` 
```
yarn
``` 
```
yarn run dev
```
Note: Make sure this all installation process is done in command prompt.

Note: Project will run on http://localhost:3000.

## Structure

I have tried my best to have standards and modular structure while developing the theme. Following sections are explaining the theme File & Folder, structure, js files struture and plugins.

### File & Folder Structure

```
app
├── public
├── scripts
├── src
	├── Components
	├── Data
	├── routes
	├── App.svelte
	└── main.js
index.html
├── .gitignore
├── package.json
├── package-lock.json
├── README.md
└── vite.config.js
```

## App.svelte

```
<script>
import { Router, Route } from "svelte-routing";

import Layout1 from "./routes/Layout1/Layout_1.svelte";
import Layout2 from "./routes/Layout2/Layout_2.svelte";
import Layout3 from "./routes/Layout3/Layout_3.svelte";
import Layout4 from "./routes/Layout4/Layout_4.svelte";
import Layout5 from "./routes/Layout5/Layout_5.svelte";
import Layout6 from "./routes/Layout6/Layout_6.svelte";
import Layout7 from "./routes/Layout7/Layout_7.svelte";
import Layout8 from "./routes/Layout8/Layout_8.svelte";
import Layout9 from "./routes/Layout9/Layout_9.svelte";
import Layout10 from "./routes/Layout10/Layout_10.svelte";
import Layout11 from "./routes/Layout11/Layout_11.svelte";
import Layout12 from "./routes/Layout12/Layout_12.svelte";
import Login from "./routes/login.svelte";
import Signup from "./routes/signup.svelte";
import Password_forget from "./routes/password_forget.svelte";

export let url = "";
</script>

<Router {url}>
  <div>
  <Route path="/"><Layout1 /></Route>
  <Route path="/layout1"><Layout1 /></Route>
  <Route path="/layout2"><Layout2 /></Route>
  <Route path="/layout3"><Layout3 /></Route>
  <Route path="/layout4"><Layout4 /></Route>
  <Route path="/layout5"><Layout5 /></Route>
  <Route path="/layout6"><Layout6 /></Route>
  <Route path="/layout7"><Layout7 /></Route>
  <Route path="/layout8"><Layout8 /></Route>
  <Route path="/layout9"><Layout9 /></Route>
  <Route path="/layout10"><Layout10 /></Route>
  <Route path="/layout11"><Layout11 /></Route>
  <Route path="/layout12"><Layout12 /></Route>
  <Route path="/login"><Login /></Route>
  <Route path="/signup"><Signup /></Route>
  <Route path="/password_forget"><Password_forget /></Route>
  </div>
</Router>
```

## Production
For production build use the below command.
```
yarn run build
```
