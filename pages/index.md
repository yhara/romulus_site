<% this.layout = 'default' %>

Steps
-----

1. npm install -g romulus

2. Create files in pages/ (and in public/, layouts/ if you want)

3. romulus[Enter] -> local server starts on http://localhost:8080/

4. romulus build [dirname=./build/] -> static html is generated

5. Deploy!

  0. Create github repository if not yet
  1. Set branch.master.remote by `git config branch.master.remote origin`
  2. Do `rm -r ./build` because `romulus deploy` uses ./build as temporary directory
  3. Finally, `romulus deploy` will create local orphan branch and pushes it to `origin/gh-pages`

