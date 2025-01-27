# Simple template

This is a basic template for a Vite + JS app. 
It is meant to be easly served on gh-pages. 

## gh-pages 
To deploy on git hub pages a sub branch of main as gh-pages.        
This sub branch will only serv the dist file. 

+ make assets
```sh
npm run build:gh-pages
```
+ add dist to the git 
```sh
git add dist -f 
```
+ commit said dist file 
```sh
git commit -m"Ajout Dist pour prod"
```
```sh
git subtree push --prefix dist origin gh-pages
```
Or
```sh
git subtree push --prefix dist template gh-pages
```
