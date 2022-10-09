### To Deploy your keys to the dev server:

- generate your key using `ssh-keygen`
- add the generated .pub key to the `playbook.yml` file in the `vars` section like so:
~~~yaml
- username: <your username>
  ssh_key: <your ssh_key id_rsa.pub> ["ssh-keygen" command to generate one]
~~~
- merge the added key with the main branch

### To ssh to the server

~~~bash
ssh <username>@78.47.231.122 -i <path_to_id_rsa>
~~~
