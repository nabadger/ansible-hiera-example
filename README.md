An Ansible example backed by Hiera
=============

Hiera
-----

Install Hiera via

    gem install hiera


Checkout this repo then:

    # Examples from ./data/default
    hiera --config hiera.yaml a_list
    hiera --config hiera.yaml a_var

    # Now using production-environment scope
    hiera --config hiera.yaml --yaml scope.yaml a_var
    hiera --config hiera.yaml --yaml scope.yaml a_production_var

