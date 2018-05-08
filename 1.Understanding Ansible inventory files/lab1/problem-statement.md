Create an ansible inventory file named `inventory`,
in the folder `practice `with a `local` host group 
and a `remote` host group.
The `local` host group should have the ip-address
of the localhost. 
The `remote` host group must have the ip-address
of the client.

After creating the file, run the command:
```
$ ansible all -i inventory --list-hosts

``` 
