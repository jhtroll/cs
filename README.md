# cs
Gen key
> ssh-keygen -t rsa -b 4096 -C "your.email@kroll.com"

Note where your key is saved
Your identification has been saved in C:\Users\user.name/.ssh/id_rsa 

Go to git bash (instead of ps or cmd), add key to ssh-agent
> eval "$(ssh-agent -s)"
> ssh-add ~/.ssh/id_rsa

Add ssh key to Github
> cat ~/.ssh/id_rsa.pub

Test ssh connection, or set correct URL
> ssh -T git@github.com
> git remote set-url origin git@github.com:jhtroll/your_repository.git
