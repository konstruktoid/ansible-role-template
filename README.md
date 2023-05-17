# Ansible role template repository

This is an [Ansible](https://www.ansible.com/) role template repository,
it contains:

- a complete Ansible role structure
- multiple GitHub actions that assists in [linting](https://ansible-lint.readthedocs.io/)
the role and managing any dependencies
- a basic [Ansible Molecule](https://molecule.readthedocs.io/en/latest/)
test environment using the [Vagrant](https://www.vagrantup.com/) driver

> **Note**
> You will need too at least update the `meta/main.yml`, `.github/CODEOWNERS`
> and `.github/workflows/issues.yml` before publishing anything.

```sh
.
├── .github
│   ├── CODEOWNERS
│   └── workflows
│       ├── issues.yml
│       ├── lint.yml
│       ├── schedlint.yml
│       ├── schedmainlint.yml
│       ├── scorecards.yml
│       └── slsa.yml
├── LICENSE
├── README.md
├── SECURITY.md
├── action-lint
│   ├── Dockerfile
│   └── entrypoint.sh
├── defaults
│   └── main.yml
├── files
│   └── .gitkeep
├── handlers
│   └── main.yml
├── meta
│   └── main.yml
├── molecule
│   └── default
│       ├── converge.yml
│       ├── molecule.yml
│       └── verify.yml
├── renovate.json
├── tasks
│   └── main.yml
├── templates
│   └── .gitkeep
├── tests
│   ├── inventory
│   └── test.yml
└── tox.ini

13 directories, 25 files
```
