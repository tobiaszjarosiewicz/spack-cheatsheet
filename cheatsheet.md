### Random commands

* Setup environment for Bash \
`source <SPACKROOT>/share/spack/setup-env.sh`

* List available compilers \
`spack compilers`

* Remove all packages from a given architecture \
`spack uninstall -a arch=<name>`

* Remove all packages from a given compiler \
`spack uninstall -a %<compiler>@<version>`

* Create a spec file for package
`spack spec -y <package_name>@<version> target=x86_64 | tee spec.yaml`
