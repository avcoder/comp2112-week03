1. Install git so you can use git bash in terminal if you want
2. Test at https://eslint.org/demo/, change ECMA to version 6, try to remove 1st error
3. Install node. `node -v` `npm -v` (yarn?)
4. Local eslint installation

   - make new folder, go into it
   - npm init -y produces a package.json
   - npm i eslint -D
   - we now have node_modules/
   - package.json eslint is under deps
   - `eslint --version`

   * `eslint --init`
   * use popular style guide > Airbnb > JSON
   * ls -a reveals .eslintrc.json
   * create index.js: `var a = "hi"`
   * `eslint index.js` reveals same errors we had at demo page

   - Install VSCode eslint extension 'eslint' by Dirk B.
   - open our folder, and bottom left corner should show errors

5. modify rules

   - lookup rule via User guide > rules: https://eslint.org/docs/rules/
   - temporary /_ eslint no-unused-vars: 1 _/
   - permanent add rules to .eslintrc.json `"rules": { "no-unused-vars": 1 }`

6. Prettier
   - install prettier extension by Esben P
   - Open user settigns, `editor.formatOnSave: true`
   - test by typing in index.js console.log ( a )

# Fetch

2. fetch
   - https://tailwindcss.com/docs/what-is-tailwind/
   ```js
   fetch(apiUrl)
     .then(function(res) {
       return res.json();
     })
     .then(function(data) {
       console.log(data);
       me = data;
       displayData();
     });
   ```
