## **[ssh-keygen](https://www.ssh.com/ssh/keygen)**

`ssh-keygen -t rsa -b 4096`

- This command will create two keys under **_~/.ssh/_** folder, and the default two keyfiles are **id_rsa** and **id_rsa.pub**.
- You can rename the default key by either **_-f_** option or during the generating process.
- You can use **_-C_** option to give the comment/label for this keyfile. This comment/label is useful in public key authentication.
- You can also give a passphrase to your existing private keyfile by using **_-P_** option.

> Examples
>
> - `ssh-keygen -t rsa -b 4096 -C 'your_email@example.com'`
> - `ssh-keygen -b 4096 -f id_rsa_example`
> - `ssh-keygen -t rsa -b 4096 -P passphrase`

## **[ssh-copy-id](https://www.ssh.com/ssh/command)**

`ssh-copy-id -i ~/.ssh/publickey user@host`

This logs into the server host, and copies keys to the server, and configures them to grant access by adding them to the **_authorized_keys_** files.

> Only the public key is copied to the server. The private key should **NEVER** be copied to another machine.

## **[ssh-agent](https://www.ssh.com/ssh/agent)**

`eval 'ssh-agent'`

`ssh-agent` is a helper program that keeps track of user's identity keys and their passphrases. The agent can then use the keys to log into other servers without having the user type in a password or passphrase again.

`ssh-add`

- `ssh-add` command is used for adding identities to the agent. By default it will add the default files _~/.ssh/id_rsa_, _~/.ssh/id_dsa_, _~/.ssh/id_ecdsa_. Otherwise, give it the name of the private key file to add as an argument.
- You can use **_-l_** option to list private keys currently accessible to the agent.

## **[SSH Config File](https://www.ssh.com/ssh/config)**

- **_Host_** Restricts the following declarations to be only for those hosts that match one of the patterns given after the keyword.
- **_HostName_** Specifies the real host name to log into.
- **_IdentityFile_** Specifies a file from which the user's identiy key is read when using public key authentication.

## **[Public Key Authentication](https://www.ssh.com/ssh/public-key-authentication)**

1. Key pair is created by **_ssh-keygen_** typically.
2. Private key stays with the user, while the public key is sent to the server by **_ssh-copy-id_** typically.
3. Server stores the public key in **_authorized_keys_** file.
4. Server will now allow access to anyone who can prove they have the corresponding private key.
