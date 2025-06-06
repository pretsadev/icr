# In Container Run (icr)

A small bash utility to run binaries in a container

# Usage
- Run supported binaries as arguments to `icr`
```bash
icr ansible --version
```
- Or symlink them to directly reference supported binaries
```bash
ln -s /path/to/icr /path/to/ansible
/path/to/ansible -- version
```

# Install
```bash
bash -c "source <(curl -s https://raw.githubusercontent.com/pretsadev/icr/main/icr-install)"
```
This will install `icr` into `.local/bin` under the users home directory. And ask to optionally install symlinks for supported binaries.

# Uninstall
Remove `icr`
```bash
rm ~/.local/bin/icr
```
If symlinks were installed, also remove them e.g.
```bash
rm ~/.local/bin/ansible
```

# Supported binaries
- Ansible
  - `ansible`
  - `ansible-galaxy`
  - `ansible-playbook`
  - `ansible-runner`
  - `ansible-test`
  - `ansible-vault`
- Antora
  - `antora`
- AWS Cli
  - `aws`
