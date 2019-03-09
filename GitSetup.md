#Installing git
`sudo apt-get install git`

#Set up personal information
`git config --global user.email "you@email.com"`
`git congig --global user.name "Your name"`

#Set up public keys
##Adding ssh key to the ssh-agent
Before adding a new SSH key to the ssh-agent which manages your keys, you should check for existing keys. You can use the command below to see if you have any existing keys.
`ls -la ~/.ssh`
If you don't see id\_rsa.pub you can generate one with the steps below. Otherwise you can use that key.
##Generating a new SSH key
Run the below command substituting your email to generate a ssh-key
`ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`
You will then be prompted to enter a file in which to save the key. Just press enter and it will be saved in the default file location.
Next you will be prompted to select a secure passphrase.
Now we will need to make sure the ssh-agent is running by using the command below.
`eval $(ssh-agent -s)`
To add the SSH private key to the ssh-agent use:
`ssh-add ~/.ssh/id_rsa`
##Adding ssh key to your github
You can use command:
`xclip -sle cli < ~/.ssh/id_rsa.pub`
to add the public key to your clipboard. If you don't have xclip installed it can be installed with command:
`apt-get -y install xclip`
Next sign into your github account and click on settings.
Then go to SSH and GPG keys
Click New SSH key.
Provide a descriptive title for this new key. Then paste the contents of your clipboard into the key field.
Click add SSH key and enter your password if prompted.
##First Clone
Now that we are all setup we can do our first clone from our repository.
`git clone git@github.com:<your github account>/<reponame>.git`

