#Docker basics

A native Linux container format that Docker calls libcontainer, as well as
the popular container platform, lxc. The libcontainer format is now the
default format.

- Linux kernel namespaces, which provide isolation for filesystems, processes and networks.
- Filesystem isolation: each container is its own root filesystem.
- Process isolation: each container runs in its own process environment.
- Network isolation: separate virtual interfaces and IP addressing between containers.
- Resource isolation and grouping: resources like CPU and memory are allocated individually to each Docker container using the cgroups, or control
groups, kernel feature.
- Copy-on-write: filesystems are created with copy-on-write, meaning they are layered and fast and require limited disk usage.
- Logging: STDOUT, STDERR and STDIN from the container are collected, logged, and available for analysis or trouble-shooting.
- Interactive shell: You can create a pseudo-tty and attach to STDIN to providean interactive shell to your container
