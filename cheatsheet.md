### Random commands

* Setup environment for Bash \
`source <SPACKROOT>/share/spack/setup-env.sh`

* List available compilers \
`spack compilers`

* Remove all packages from a given architecture \
`spack uninstall -a arch=<name>`

* Remove all packages from a given compiler \
`spack uninstall -a %<compiler>@<version>`

* Create a spec file for package \
`spack spec -y <package_name>@<version> target=x86_64 | tee spec.yaml`

* Edit config (~/.spack/config.yaml): \
`spack config edit config`

### Installing package
* Specify architecture \
`spack install <package_name> target=x86_64`

* Specify compiler \
`spack install <package_name> %compiler`

* Specify explicit dependency \
`spack install <package_name> ^<dependency>@<version>`
