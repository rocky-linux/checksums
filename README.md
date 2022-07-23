# checksums

This repository contains checksums for images, ISO's, and so on for Rocky Linux.
They are sorted by version into various directories.

| Release            | Purpose                        |
|--------------------|--------------------------------|
| rocky-linux-8      | Rocky Linux 8                  |
| rocky-linux-9      | Rocky Linux 9                  |
| rocky-linux-rc     | Rocky Linux Release Candidates |
| images             | Rocky Linux Images per release |

This repository is mirrored here: https://git.resf.org/rocky-linux/checksums

# Why this repository?

One of the goals of this repository is to be a main point of reference for all
checksums for our images, regardless of release. It can also be a historical
reference as well because all versions will be available.

This repository is also a result of the following things:

* Keykeeper (part of the peridot build system) does not sign arbitrary files
or artifacts outside of the build system

* We are planning to move Rocky Linux 8 into the new build system, and along
with it, the keys that sign the packages and repository metadata

* Some users would rather have a place they can go to that is outside of the
mirror(s) to verify the signatures are valid and the checksums actually match
what they claim.

# So the commits are signed, how do I verify?

To verify our signature, click on "commits", click on the green "Verified"
button where you will see a GPG key ID. You can then search for this ID at
any of the following:

https://keys.openpgp.org
https://keyserver.ubuntu.com
