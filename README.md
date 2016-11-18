# ansible-consul-replicate

## Synopsis

```yml
- hosts: all
  vars:
    consul_replicate_consulhost: 'https://consul.tld.com'
    consul_replicate_additional_opts:
      - '-foo bar'
  roles:
    alvaroaleman.consul-replicate
```

## Role Variables

* ``consul_replicate_version``: Version of consul-replicate to install (default: ``0.2.0``)
* ``consul_replicate_bindir``: Directory in which to create subdirs for each consul-replicate version and a link to the current version (default: ``/usr/local/bin``)
* ``consul_replicate_consulhost``: Address of consul (default: ``127.0.0.1:8500``)
* ``consul_replicate_additional_opts``: Addiotional CLI opts to pass to consul-replicate (default: ``[]``)

## Contributing

If you want to contribute to this repository please be aware that this
project uses a [gitflow](http://nvie.com/posts/a-successful-git-branching-model/)
workflow with the next release branch called ``next``.

Please fork this repository and create a local branch split off of the ``next``
branch and create pull requests back to the origin ``next`` branch.

## License

AGPLv3

## Author information

* Alvaro Aleman

<!-- vim: set nofen ts=4 sw=4 et: -->
