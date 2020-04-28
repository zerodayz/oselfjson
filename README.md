# oselfjson

This repository contains [a script](generate_aliases.py) to generate hundreds of
convenient shell aliases for openstack client, so you no longer need to spell out every single
command.

An example shell alias created from command/flags permutation looks like:

    alias onesfjson='openstack network show -f json'

### Examples

Some of the generated aliases are:

```
alias oses='openstack server show'
alias ones='openstack network show'
alias ofls='openstack flavor show'
alias osus='openstack subnet show'
alias oros='openstack router show'
alias osts='openstack stack show'
alias ostres='openstack stack resource show'
alias osel='openstack server list'
alias onel='openstack network list'
alias ofll='openstack flavor list'
alias osul='openstack subnet list'
alias orol='openstack router list'
alias ostl='openstack stack list'
alias ostrel='openstack stack resource list'
alias osec='openstack server create'
alias onec='openstack network create'
alias oflc='openstack flavor create'
alias osuc='openstack subnet create'
alias oroc='openstack router create'
alias ostc='openstack stack create'
alias oserm='openstack server delete'
alias onerm='openstack network delete'
alias oflrm='openstack flavor delete'
alias osurm='openstack subnet delete'
alias ororm='openstack router delete'
alias ostrm='openstack stack delete'
alias osesfyaml='openstack server show -f yaml'
alias onesfyaml='openstack network show -f yaml'
alias oflsfyaml='openstack flavor show -f yaml'
alias osusfyaml='openstack subnet show -f yaml'
alias orosfyaml='openstack router show -f yaml'
alias ostsfyaml='openstack stack show -f yaml'
alias oselfyaml='openstack server list -f yaml'
alias onelfyaml='openstack network list -f yaml'
alias ofllfyaml='openstack flavor list -f yaml'
...
```

### Syntax

```
('o') = ('openstack')
('se') = ('server')
('ne') = ('network')
('s') = ('show')
```

For example

`osel` => `openstack server list`  
`onel` => `openstack network list`

### Installation

You can directly download the [`.openstack_aliases` file](https://raw.githubusercontent.com/zerodayz/oselfjson/master/.openstack_aliases)
and save it in your $HOME directory, then edit your .bashrc/.zshrc file with:

```
[ -f ~/.openstack_aliases ] && source ~/.openstack_aliases
```

This project wouldn't be possible without [@ahmetb](https://twitter.com/ahmetb), Thank you!

-----

This is not official OpenStack project.
