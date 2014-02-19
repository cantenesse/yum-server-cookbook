# yum_server cookbook

# Requirements

# Resources/Providers

## Examples

```
yumrepo 'myorg' do
	document_root /var/www
	alias /myorg/yum
	webserver apache
end
```

This will install apache, create a site with a virtual host aliasing /myorg/yum to /var/www/blah and create repo metadata

# Attributes
default[:yum_server][:webserver] = 'apache'
default[:yum_server][:reponame] = 'yum'
default[:yum_server][:document_root] = '/var/www'
default[:yum_server][:alias] = 'yum'

# Recipes
default.rb - Builds a 

# Author

Author:: Chris Antenesse (<chris@antenesse.net>)
