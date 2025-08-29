---
title: dpkg-archive
section: 1
header: User Commands
footer: dpkg-archive(1)
date: 2025-08-11
author:
    Michael Schaecher <michaelschaecher@mlstidbits.com>
---

# SYNOPSIS

`dpkg-archive`

`file`: $HOME/path/to/archive

# DESCRIPTION

Manages Debian/Ubuntu package archives easily, with a focus signing and verification.

# CONFIGURATION

The configuration file is located at `$HOME/patch/to/archive/config.yaml`. It contains the following fields:

```yaml
key:
  enable: true
  name: dpkg-archive
```
## KEY

The `key` section allows you to enable or disable the use of a GPG key for signing and verifying packages in the archive. The `name` field specifies the name of the key to be used.

---

Example: name: `MLS Tidbits`

---

Default: enable: `true`, name: `dpkg-archive`

## RElEASE

The `release` section allows you to specify the release information for the archive. It contains the following fields:

---

Origin: The origin of the archive, typically the name of the organization or project.

---

Label: The label for the archive, which is usually the same as the origin.

---

Suite: The suite of the archive, such as `stable`, `testing`, or `unstable`.

---

codename: The codename for the release, which is a short identifier for the version of the archive.

---

architectures: A list of supported architectures for the packages in the archive.

---

components: A list of components in the archive, such as `main`, `contrib`, or `non-free`.

---

description: A brief description of the archive.

## MAINTAINER

The `maintainer` section allows you to specify the maintainer information for the archive. It contains the following fields. This is offend the company/organization name plus the email address of the maintainer.

---

Name: The name of the maintainer.

---

Email: The email address of the maintainer.

# SEE ALSO

`dpkg(1)`, `apt(8)`, `apt-get(8)`

# LICENSE

Copyright (c) 2025 Michael Schaecher <michaelschaecher@mlstidbits.com>

Copyright (c) 2025 MLS Tidbits <contact@mlstidbits.com>
