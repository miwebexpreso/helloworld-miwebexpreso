GitHub / Git 2025

DESKTOP APP GITHUB (Basic Level Users)
https://docs.github.com/es/get-started/start-your-journey/hello-world

_________________________
12345678901234567890

GIT command line (Medium Level Users)
https://docs.github.com/es/get-started/using-git/about-git
https://docs.github.com/es/get-started/using-git/about-git
https://docs.github.com/es/get-started/using-git/about-git


https://docs.github.com/es/get-started/onboarding/getting-started-with-your-github-account#1-learning-git

https://docs.github.com/es/get-started/git-basics/about-remote-repositories


GIT CREDENTIAL MANAGER application
Git Credential Manager repository

https://github.com/git-ecosystem/git-credential-manager

Git Credential Manager (GCM) is a secure Git credential helper built on .NET that runs on Windows, macOS, and Linux. It aims to provide a consistent and secure authentication experience, including multi-factor auth, to every major source control hosting service and platform.

GCM supports (in alphabetical order) Azure DevOps, Azure DevOps Server (formerly Team Foundation Server), Bitbucket, GitHub, and GitLab. Compare to Git's built-in credential helpers (Windows: wincred, macOS: osxkeychain, Linux: gnome-keyring/libsecret), which provide single-factor authentication support for username/password only.

GCM replaces both the .NET Framework-based Git Credential Manager for Windows and the Java-based Git Credential Manager for Mac and Linux.

https://github.com/git-ecosystem/git-credential-manager/blob/release/docs/install.md

https://github.com/git-ecosystem/git-credential-manager/releases/tag/v2.6.1

How to use

Once it's installed and configured, Git Credential Manager is called implicitly by Git. You don't have to do anything special, and GCM isn't intended to be called directly by the user. For example, when pushing (git push) to Azure DevOps, Bitbucket, or GitHub, a window will automatically open and walk you through the sign-in process. (This process will look slightly different for each Git host, and even in some cases, whether you've connected to an on-premises or cloud-hosted Git host.) Later Git commands in the same repository will re-use existing credentials or tokens that GCM has stored for as long as they're valid.

https://github.com/git-ecosystem/git-credential-manager/blob/release/docs/usage.md

---------

MANAGING YOUR PERSONAL ACCESS TOKENS
https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens

La clasica, creas el token (classic y fine-grained) y no los copias con todo y que te dicen que no lo volverás a ver cuando lo creas. Regeneras nuevamente ambos tokens.

Se crearon los tokens para cuentas GitHub miwebexpreso y mapalmalemus

NOTA:  Funcionalidad de dos usuarios GitHub con un mismo usuario MacOS

miwebexpreso GitHub User
Safari Browser para GitHub Web
Terminal Console para git commands 
GIT CREDENTIAL MANAGER para autenticación GitHub
(GCM package Mac installed)

mapalmalemus GitHub User
Safari Browser para GitHub Web
Desktop App GitHub (autenticación por default al instalar)
Terminal Console para git commands 
MANAGING PERSONAL ACCESS TOKESN para autenticación GitHub

-------

Ejemplo: Contribuir con un repositorio existente

# download a repository on GitHub to our machine
# Replace `owner/repo` with the owner and name of the repository to clone
git clone https://github.com/owner/repo.git

# change into the `repo` directory
cd repo

# create a new branch to store any new changes
git branch my-branch

# switch to that branch (line of development)
git checkout my-branch

# make changes, for example, edit `file1.md` and `file2.md` using the text editor

# stage the changed files
git add file1.md file2.md

# take a snapshot of the staging area (anything that's been added)
git commit -m "my snapshot"

# push changes to github
git push --set-upstream origin my-branch

------

Ejemplo: Comienza un repositorio nuevo y publícalo en GitHub
Primero, necesitas crear un repositorio en GitHub. Para más información, consulta Hola mundo. No inicialice el repositorio con un archivo Léame, .gitignore o de licencia. Este repositorio vacío esperará tu código.

# create a new directory, and initialize it with git-specific functions
git init my-repo

# change into the `my-repo` directory
cd my-repo

# create the first file in the project
touch README.md

# git isn't aware of the file, stage it
git add README.md

# take a snapshot of the staging area
git commit -m "add README to initial commit"

# provide the path for the repository you created on github
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY-NAME.git

# push changes to github
git push --set-upstream origin main



INICIALIZACIÓN DE REOPOSITORIO HELLO WORLD SIMPLE o VACIO que espera código. Cuando se crea en GitHub Web te proporciona las siguiente secuencia de comandos para subir tu repositorio (ESTO ES LO QUE REQUERIA PARA MPLAB X IDE) 

echo "# helloworld-miwebexpreso" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/miwebexpreso/helloworld-miwebexpreso.git
git push -u origin main

----------

git remote add origin https://github.com/miwebexpreso/helloworld-miwebexpreso.git
git branch -M main
git push -u origin main

---------

Ejemplo: Contribuye con una rama existente en GitHub

En este ejemplo se da por hecho que ya tienes un proyecto llamado repo en la máquina y que se ha insertado una rama nueva en GitHub desde la última vez que se realizaron los cambios localmente.

# change into the `repo` directory
cd repo

# update all remote tracking branches, and the currently checked out branch
git pull

# change into the existing branch called `feature-a`
git checkout feature-a

# make changes, for example, edit `file1.md` using the text editor

# stage the changed file
git add file1.md

# take a snapshot of the staging area
git commit -m "edit file1"

# push changes to github
git push

---------

GITHUB del GITHUB
https://github.com/github
https://github.com/orgs/github/repositories?type=all
https://github.com/github/roadmap

_________________________
12345678901234567890

GIT command (High Level Users)

https://git-scm.com/docs
https://git-scm.com/docs/gitcredentials#_custom_helpers

