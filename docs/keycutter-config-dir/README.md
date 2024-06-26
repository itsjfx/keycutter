# Keycutter Configuration Directory

The Keycutter configuration directory, located at `~/.keycutter` by default, is the central repository for all configuration files and keys managed by the Keycutter tool.

This directory contains configurations for git and SSH, along with a general config file (not yet used), facilitating a modular and organised approach to managing access and identity across different services and platforms.

It assists users by containing all the configuration files and keys in one place, making it easier to review and maintain.

## Example Config Generated by Keycutter

The Keycutter configuration directory consists of the following components:

```
$ tree ~/.keycutter
/home/m/.keycutter
├── git
│   ├── allowed_signers                  # Verify commits signed with SSH Keys
│   ├── config.d
│   │   └── github-alexdoe-work          # Git config associated with this key
│   └── gitconfig-keycutter              # Conditionally includes config.d files
└── ssh                     
    ├── config.d
    │   └── github-alexdoe-work          # SSH configuration for key
    └── keys                             
        ├── yk01@github-alexdoe-work     # SSH private key
        └── yk01@github-alexdoe-work.pub # SSH Publivc Key
```

You can view the files in [example_dot_keycutter/](example_dot_keycutter/).
