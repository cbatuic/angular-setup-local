# How to setup Git in Angular project locally and Commit to Github?
See original post [here](https://www.freakyjolly.com/setup-git-in-angular-project-commit-changes/).

1. Install requirements
  * [NodeJS](https://nodejs.org/en/download/)
  * [Git](https://git-scm.com/downloads)
2. Verify installation and Setup project directory

```bash
> node --version
> npm --version
> git --version
> mkdir angularsetup
> cd angularsetup
```

3. Create a new Angular project and open with VisualStudio code

```bash
> npm install -g @angular/cli
# wait
> ng new lastname-angularsetup
# wait
> cd lastname-angularsetup
> code .
```

4. Run the application

```bash
> ng serve --open
# The --open (or just -o) option automatically opens your browser to http://localhost:4200/.
```

5. Execute Git Command to Commit locally

```bash
# open new terminal (command prompt)
> cd angularsetup/lastname-angularsetup
> git init
> git config user.email "youruicemail@uic.edu.ph"
> git config user.name "yourgithubusername"
> git status
> git add .
> git commit -m "initial commit by lastname"

```

6. Create New Github Repository entitled ***lastnameangularsetup***. Make the repo ***"public"*** and ***"Add Readme.md"*** not selected. Create the repo and copy the commands under the ***"... push an existing repository from the command line"***

7. Add remote url and push your codes

```bash
> git remote add origin https://github.com/[yourgithubusername]/lastnameangularsetup.git
> git push -u origin master
```

8. **That’s it now you have successfully committed your files on GitHub repository!** 

Note: Now when you will make modifications to any files or folders, follow the same procedure in step 4 above to commit your changes.

```bash
> git status
> git add .
> git commit -m "changes in the index.html"
> git push origin
```

## Congratulations! Off to the next task.
