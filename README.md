# PyAnsys all-members team
Repository for updating the pyansys/all-members team automatically

## How does it work?
This repository basically contains a simple Python script ``update_team.py``. Within this
script, there are two main variables which a user must take into account:

* ``my_pat``: this variable will basically include your personal authentication token in order
to interact with GitHub (using PyGitHub). You can also make use of the automated mechanism, by which
the script will search for an environment ariable named ``TOKEN`` which should contain your PAT.
* ``my_org``: the organization whose team ``all-members`` we want to update.

In order to run it, simply modify these values and run:

```bash
    python update_team.py
```

Bare in mind that this specific version of the script has already set up the ``my_org`` variable
to ``pyansys``, since it the organization for which this repository is oriented.

## Requirements

In order to run the previous script, one only needs to install ``pygithub``. In order to ease the
user its installation, we have created a requiorements file: ``requirements.txt``. You can install
the latest version of the package by doing as follows with the ``pip`` package manager:

```bash
    pip install -r requirements.txt
```