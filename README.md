The problem appears to be related to Visual Studio and `npx` command.

# Used Environment

OS: Windows 10

IDE: Visual Studio 2019
```
> nvm version  
1.1.7

> npx -v
7.19.1

> npm -v
7.19.1

> node -v
v16.5.0
```

# Repro steps
Try the following steps using Visual Studio (at least for step 3).

0. Clone repo
1. Install dependencies
```sh
# run following in root of cloned directory
npm install
```
2. Create new file (or make some changes to commit)
3. Commit changes using the Visual Studio - Git Changes panel

Should observe following error in Visual Studio on Git Changes panel (but not in VS Code).
```
/usr/bin/env: 'bash': No such file or directory
husky - pre-commit hook exited with code 127 (error)
```
