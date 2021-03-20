# Usefull

Use below to save project in local and remote server.

```bash
git add . && git commit -m 'Hello World' && git push -u origin master

"save": "git add . && git commit -m '🔹' && git push -u origin master"
```

If we add something to .gitignore file like node\_modules but we have already pushed the node\_modules to GitHub then we have to use below git command then add - commit - push changes to GitHub

```bash
git rm -r --cached . 
```



```text
git remote -v
git remote set-url origin git@github.com
```

```text
// update all major updates for all the packages

// remove node_modules & package-lock.json
// npm install -g npm-check-updates

npx rimraf ./**/node_modules
rm package-lock.json
ncu -u
npm cache verify
npm install
```

```javascript
ncu -g // for global package updates
```

[https://heroicons.dev/](https://heroicons.dev/) tailwindui icons \(svg copy/paste for small projects that do not need to require fontawesome\)

[https://simpleicons.org/](https://simpleicons.org/) \(svg company logo icons\)

{% embed url="https://www.flaticon.com/" %}

```javascript
// defining explicit origin example
server.use(cors({ credentials: true, origin: 'http://localhost:3000' }))
```

Github README Markdown [https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)

tracert google.com \(example\)



