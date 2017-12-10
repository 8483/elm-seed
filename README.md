# elm-seed

- **server/** (backend goes here)
- **app/** (elm app)
 - ~~elm-stuff~~
 - ~~elm-package.json~~
 - Main.elm
- **public/** (final product)
 - css/
    - bootstrap.css
    - style.css
 - js/
    - jquery.js
 - index.html
 - ~~main.js~~

Note: ~~ignored files~~

# Install
```bash
sudo npm install -g elm # Normal install
sudo npm install --unsafe-perm -g elm # If npm gives you permission errors.
```

# Build/Compile
```bash
cd app # Move into the app directory.
elm-make Main.elm --output=../public/main.js # Compile the elm code from Main. elm into javascript, and put it in the public folder as main.js
```

The result from this is the creation of:
- `elm-stuff` - Holds the dependecies, like `node_modules`.  
- `elm-package.json` - Lists the dependecies, like `package.json`.  
- `main.js` - The transpiled elm code, to be used in `index.html`.