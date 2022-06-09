
# ubuntu-setup-configs

some scripts and configfiles for comfy operations.

You have to clone this repository to your (Ubuntu-) Machine and start either the desktop or Serverscript:

`git clone https://github.com/datenklo/ubuntu-setup-configs.git`
`cd ubuntu-setup-configs`
`./get-server-config`

OR

`./get-desktop-config`

(Desktop has additional Apps for install (VMWare Workstation with Kernelfix and Visual Studio Code)

# The Equivalent to ssh-copyid does not Exist in Windows. But there is help, just use this snippet

First create a Keypair with the usual ssh-keygen.

Then use_

`type $env:USERPROFILE\.ssh\id_rsa.pub | ssh {USER@HOST} "cat >> .ssh/authorized_keys"`

Now Test Connection (Does NOT Work with ESXI-Servers!) with "ssh USER@HOST"

On ESXI you have to change the path a little bit:

`type $env:USERPROFILE\.ssh\id_rsa.pub | ssh {USER@HOST} "cat >> /etc/ssh/keys-{USER}/authorized_keys"`
