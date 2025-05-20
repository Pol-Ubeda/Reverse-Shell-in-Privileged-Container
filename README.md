# Reverse-Shell-in-Privileged-Container

For educational purposes only.

This is a simple script one can run in a privileged container to gain a reverse shell on the system hosting the container.

For this particular exploit one needs the SYS_ADMIN capability, which can be checked using ```capsh --print```.

It uses the cgroups filesystem, in particular it's ```release_agent``` file functionality in order to execute the ```/exploit``` we create.
