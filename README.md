
# ubuntu-setup-configs

some scripts and configfiles for comfy operations

# Some Hint

## The Equivalent to ssh-copyid does not Exist in Windows. But there is help, just use this snippet

First create a Keypair with the usual ssh-keygen.

Then use_

type $env:USERPROFILE\.ssh\id_rsa.pub | ssh {USER@HOST} "cat >> .ssh/authorized_keys"

Now Test Connection (Does NOT Work with ESXI-Servers!) with "ssh USER@HOST"
