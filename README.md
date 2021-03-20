# Usefull

```javascript
"save": "git add . && git commit -m '🔹' && git push -u origin master"
```

```bash
# If we add something to .gitignore file like node_modules 
# but we have already pushed the node_modules to GitHub 
# then we have to use below git command then add - commit - push changes to GitHub
git rm -r --cached . 
# then save, npm run save-alpha etc.
```

```bash
git remote -v
git remote set-url origin git@github.com
```

```bash
# update all major updates for all the packages

# remove node_modules & package-lock.json
# npm install -g npm-check-updates

npx rimraf ./**/node_modules
rm package-lock.json
ncu -u
npm cache verify
npm install
```

```javascript
ncu -g // for global package updates
```

```javascript
// defining explicit origin example
server.use(cors({ credentials: true, origin: 'http://localhost:3000' }))
```

