# DeveloperToolKitGitBash
Let’s begin, my path “Leo Developer Toolkit through Git Bash”

*To paste command press Shift+Win+Insert (Windows)*

## What will we need (Preparation) :
1. Install [Git Bash (Follow instructions for Windows)](https://git-scm.com/downloads)
2. Install [the components you need for building C and C++ apps](https://visualstudio.microsoft.com/vs/features/cplusplus/)

## What do we do:

### 1. Download and install Leo
1.1 Install Rust
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

![1 and enter](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/b3e54dd5-90ae-46d9-82ab-b150d97c917d)

Press **1** and **Enter**

![enter](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/902f9aa5-feaa-4386-9ebe-7bad354eafe6)

Press Enter again

1.2 Download the source code
```
git clone https://github.com/AleoHQ/leo
```
![clone](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/91772ddf-0af6-46e0-91e4-410955df3908)
```
cd leo
```
![cd leo](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/037e96fb-054e-4ba8-bace-b6310408fec7)

1.3 Install Leo

```
cargo install --path .
```

After entering this command, the Leo installation process will begin

![install](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/026ac1d2-5a35-43ee-a83a-fe3a827817e1)

Wait for it to finish, the process takes 5–10 minutes depending on the power of your computer

1.4 Try writing `leo help` command

![leo help](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/924b2fca-9f1e-4a98-96b4-ca53b84a6d49)

If everything looks like this, congratulations, leo is installed!

## 2. Working with Leo
2.1 Create a new wallet
```
leo account new
```

or you can import your current wallet
```
leo account import YOUR_Private_Key
```

2.2 Continue in your exsiting terminal window and type `leo example`

![leo example](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/1f667f97-9165-4379-8910-6d55c08a4a0e)

2.3 We'll try TicTacToe
```
leo example tictactoe
```

![example tictactoe](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/249c2d3b-2554-4a80-8c77-bd22d94bc8f0)

2.4 You can run and see the example in action
```
cd tictactoe
```

and run
```
leo run new
```
![leo run new](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/d66ef945-a6a8-46dd-a90a-f7cf37bcc7f1)

## 3. Push your Leo app to GitHub
3.1 Initializing a Git repository
```
cd tictactoe
```
```
git init -b main
```
```
git add .
```
![git init add .](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/9a573e5b-7b6c-46d5-9921-2701ff764428)

3.2 Before committing, we need to add your email
write the command in the terminal
```
git config --global user.email mail@.com
```
**where mail@.com is your email adress*
```
git config --global user.name your_username
```
**where your_username is your username)

3.3 Now you can commit
```
git commit -m "My First commit"
```
![First Commit](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/1204d955-1867-4f13-8537-1764b7e48832)

3.4 Adding a local repository to GitHub using Git
Create a new repository on [Github](https://github.com/new)

![new repo](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/d8726192-9ad6-4e84-8162-f7ceeb404c02)

Type your repository name (you can call it whatever you want) and press Create repository (to avoid errors, do not initialize the new repository with README, license, or gitignore files)

3.5 Copy the link to your repository

![Copy the link](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/54bc71da-a581-437b-a2e3-ef1f8ecefb7b)

3.6 Continue in your existing terminal window and type
```
git branch -m main
```
```
git remote add origin YOUR_REPOSITORY_LINK
```
```
git remote -v
```
```
git push -u origin main
```

![After push](https://github.com/HausenUA/DeveloperToolKitGitBash/assets/107180551/fba93cb3-e414-4dce-98d0-1de1c8a837a2)

## 4. Congratulations, you can view your repository via your link or in your GitHub profile
[An example of what I came up with when I created this guide](https://github.com/HausenUA/tictactoe)


## Continue your Leo journey
Check out the following resources:

- [Aleo developer docs](https://developer.aleo.org/getting_started/)
- See Aleo’s SDK in action at [aleo.tools](https://aleo.tools/)
- Play around with Leo in the browser with [Leo Playground](https://play.leo-lang.org/)
- Learn Leo syntax, functions, and best practices with the [Leo’s language guide](https://developer.aleo.org/leo/language)
- Deploy and Execute Leo applications on-chain with our [Deploy and Execute Demo](https://developer.aleo.org/testnet/getting_started/deploy_execute_demo)
- See Aleo’s testnet live and other Leo developer’s applications via an explorer such as [Haruka’s Program Registry](https://explorer.hamp.app/programs) or [aleo.network](https://www.aleo.network/)


