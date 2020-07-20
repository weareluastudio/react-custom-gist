<div align="center">
<img src='https://blog.wearelua.com/images/general/logo.png' title='LUA Logo' height='70' />
<h1>LUApp® | react-custom-gist</h1>
<img src='https://img.shields.io/npm/v/react-custom-gist?style=for-the-badge' title='NPM Version'/>

<img src='https://img.shields.io/badge/LUABuild-react-green?style=for-the-badge' title='Build'/>

<img src='https://img.shields.io/badge/PoweredBy-LUADevStudio-blue?style=for-the-badge' title='Powered By'/>

<p>React-custom-gist its a embedded gist on a custom iFrame with syntax color theme. You can select 'Monokai | Solarized | Chaos | Cobalt | Idle Fingers | Obsidian ...' and many others as theme</p>
</div>

----

## 👌 Share awesome gist

yarn:
```
    yarn add --save react-custom-gist
```

npm:
```
    npm i --save react-custom-gist
```

## ✍️ Using
The default thme is Monokai
```javascript
    // App.tsx
    import React from 'react';
    import Gist from 'react-custom-gist'

    const App:React.FC = () => {
        const url:string = 'your gist url'
        return <Gist src={url}/>
    }

    export default App
```

choose your theme

```javascript
    // App.tsx
    import React from 'react';
    import Gist from 'react-custom-gist'

    const App:React.FC = () => {
        const url:string = 'your gist url'
        return <Gist src={url} theme='solarized-light'/>
    }

    export default App
```
choose your styles

```javascript
    // App.tsx
    import React from 'react';
    import Gist from 'react-custom-gist'

    const App:React.FC = () => {
        const url:string = 'your gist url'
        return <Gist src={url} theme='solarized-light' style={{border:'none'}}/>
    }

    export default App
```
And thats it!, just add your git url to render a gist on your app.
A special feature of this gist its the content based height.

## 🛠 Props

| Name  | Type                                                                                                                                                                | Default   | Optional |
|-------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------|----------|
| src   | string                                                                                                                                                              |           | false    |
| style | CSSProperties                                                                                                                                                       | undefined | true     |
| theme | monokai<br>solarized-light<br>solarized-dark<br>chaos<br>cobalt<br>idle-fingers<br>obsidian<br>one-dark<br>pastel-on-dark<br>terminal<br>tomorrow-night<br>twilight | monokai   | true     |

You can see all themes and styles [here](https://lonekorean.github.io/gist-syntax-themes/)

### LICENSE MIT
All rights reserved LUA Development Studio ®
