To start a jekyll blog on github pages :
1. Create a new repository on github
2. Install jekyll
ruby -v
gem -v
sudo gem install jekyll
jekyll -v

3. Create a jekyll site
jekyll new myjekyllblog
jekyll serve --watch


4. Change the configurations
Your Jekyll blog’s configurations reside in the _config.yml file. When you install Jekyll it comes with a default config. Open the file in a code editor and change the values.

5. Add Blog Posts
year-month-date-{slug}.md

6. Push the site live
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/myjekyllblog/myjekyllblog.github.io
git push origin master
