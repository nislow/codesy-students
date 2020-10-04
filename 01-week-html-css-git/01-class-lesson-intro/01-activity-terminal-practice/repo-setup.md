# Instructions to setup the codesy-students repo on your computer:

1. Ensure first that you have ssh authentication set up on your computer for github, to test this run this command: `ssh -T git@github.com`

2. If you get a permissions error like: `Permission denied (publickey)` running the ssh test command in step 1. then you need to set up the ssh authentication using these links as guide: https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent and https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account. __NOTE:__ When generating the ssh and you are prompted for file location, press enter. When prompted for passphrase, skip by press enter. You do not need to add your SSH key to the ssh-agent.

3. If you have your ssh key setup but you get an error like ssh: `connect to host github.com port 22: Connection timed out` or `ssh: connect to host github.com port 22: Connection refused` then you need to use ssh via port 443 (usually it is port 22, but replacing the ssh config to use 443 works as it is a standard port that is accepted by most computer/firewall configurations). To set this up follow the instructions on this link: https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/using-ssh-over-the-https-port. __NOTE:__ first test that you can use this method for ssh by running the test command in the link. You should get: `Hi (your github username e.g. bilaal-s)! You've successfully authenticated, but GitHub does not provide shell access`. Then carry on with the remaining steps in the guide, making sure that you create a file called `config` (no extensions) in your ssh folder (`~/.ssh`). you can do that by running the command: `touch ~/.ssh/config` (this is the recommended approach) __OR__ manually by going to the file explorer, navigating to `C:\Users\(your computer username)\.ssh` on windows or `/Users/(your computer username)/.ssh` on mac (you need to make sure you can see hidden files/folders for both mac and windows) and create a file called `config` . Once you have created the config file, you can carry on following the instructions in the guide, taking the contents of for the config file from the guide and putting it in your own config file. After that, test again and your issues should be resolved.

4. __NOTE: You can skip this step if you have already forked.__ With ssh setup you can now fork the `codesy-students repo`, to do so visit https://github.com/bilaal-s/codesy-students and click the 'fork' button near the top.

5. Before continuing create a folder in your home directory called codesy with the command `mkdir ~/codesy`.

6. Go into that directory with the command `cd ~/codesy`

7. __IMPORTANT:__ Next, go to your own fork of the codesy-students repo by clicking the profile icon in the to right, then clicking 'Your repositories', then clicking codesy-students.

8. Click the green 'Code' button, choose SSH then copy the url with the copy button next to the URL.

9. Go back to the terminal, make sure you are still in the `~/codesy` folder by running the command: `pwd`. It should should show up with something like `/home/<YOURUSERNAME>/codesy` or `/Users/<YOURUSERNAME>/codesy` or similar.

10. Type `git clone` then paste the URL you copied to get a copy of your fork of the `codesy-students` repo onto your computer, the command should look something like: `git clone git@github.com:<YOURUSERNAME>/codesy-students.git`. __NOTE:__ <YOURUSERNAME> should be your own GitHub username.

11. Finally, go into the `codesy-students` folder with: `cd codesy-students`.

12. After you have completed the above steps the final step is to setup a remote to keep my repo in sync with yours, the guide for that is: https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/configuring-a-remote-for-a-fork. __IMPORTANT:__ ensure you replace the url in step 3 with my (instructor) version of the repo, the URL is: `git@github.com:bilaal-s/codesy-students.git`, so the complete command for step 3. of the guide will look like: `git remote add upstream git@github.com:bilaal-s/codesy-students.git`.