//Git global setup

git config --global user.name "chiyanglin"
git config --global user.email "chiyanglin@gmail.com"


// in git lab have test-gitlab.git
//------------------------------------------------------------------------------
//Command line instructions
//You can also upload existing files from your computer using the instructions below.
//
// Usage 1 : Create a new repository
git clone https://gitlab.com/chiyanglin/test-gitlab.git
cd test-gitlab
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master

// Usage 2 :Push an existing folder
cd existing_folder
git init
git remote add origin https://gitlab.com/chiyanglin/test-gitlab.git
git add .
git commit -m "Initial commit"
git push -u origin master

// Usage 3 :Push an existing Git repository
cd existing_repo
git remote rename origin old-origin
git remote add origin https://gitlab.com/chiyanglin/test-gitlab.git
git push -u origin --all
git push -u origin --tags


// in git hub have test-github.git
//-----------------------------------------------------------------------
// Usage 1 :create a new repository on the command line
echo "# test-github" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/chiyanglin-AStar/test-github.git
git push -u origin main

// Usage 2 :create push an existing repository from the command line
git remote add origin https://github.com/chiyanglin-AStar/test-github.git
git branch -M main
git push -u origin main

