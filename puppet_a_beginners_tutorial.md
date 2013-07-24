###Puppet: A Beginners Tutorial


https://github.com/ghoneycutt/oscon2013 - Extra code for the session
Garrett Honeycutt - gh@garretthoneycutt.com

github.com/ghoneycutt has a ton of his own modules

forge.puppetlabs.com - puppet modules already pre-written
You should have one base install for all servers on your network.  No matter what the server is.
The whole concept of puppet is to have a defined state and get you and keep you there.
Catalog - comprehensive list of resources on system

setup script he sent shows a lot of errors.  running puppet agent -t seems to work though.

facter command gets data about a system

set your own command by setting environment variables
export FACTER_myfact=oscon2013
facter myfact

puppet resource will let you see what is going on with a specific service:
     puppet resource service postfix
     puppet resource user root

you can make changes with puppet resource:
     puppet resource service postfix ensure=stopped

docs.puppetlabs.com/references/stable/type.html
puppet type reference page ^

config file: /etc/puppet/puppet.conf or puppet config print

semver.org - semantic versioning read this - very short read and super important for everything.

site manifest: /etc/puppet/manifests/site.pp

puppet master is a cpu bound system - to scale it out, throw more cores at it

puppet labs style guide 

puppet-lint - style checker

add puppet parser and puppet lint into your pre-commit hooks to make sure everything is great

puppet help <command> will give you help on each specific command

check motd init.pp for variables in package and pulling in facts

you have to create the relationships between the resources in the puppet files, it doesn't do it for you.

hiera is hierarchy setup tool to differentiate between all kinds of environments
     much more complex here, and I don't think he is going to go into this enough…

it looks like hiera is the way to customize a lot of what will be changed - need to get a lot more information on this.

should store all configurations and also the hiera stuff in version control.

should run the agent in cron, but manage when it checks in using puppet
