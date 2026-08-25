# day 13: dnf-yum
1. **dnf update** — refreshes and upgrades packages on RPM-based systems (Fedora, RHEL, Amazon Linux) in one step, unlike APT which splits that into `update` then `upgrade`.

2. **dnf install** — installs a package by name along with its dependencies, the RPM-world equivalent of `apt install`.

3. **dnf remove** — uninstalls a package. On DNF-based systems this generally behaves closer to APT's `purge` than its `remove`.

4. **dnf search** — searches package names and descriptions for a keyword, same purpose as `apt search` but against RPM repositories.

5. **yum install** — the older command-line tool that `dnf` was built to replace. Still shows up on older RHEL/CentOS systems, and `dnf` accepts most of the same syntax.

6. **rpm -qa** — lists every RPM package currently installed on the system, which is how I'd confirm an install actually landed.

7. **snap install** — installs a package as a Snap, a self-contained format that bundles its own dependencies and works across different distributions rather than being tied to APT or DNF/YUM.

8. **add-apt-repository** — adds a new software source to APT's list of repositories, needed when a package isn't available in the default ones.

9. **dpkg -i** — installs a package directly from a local `.deb` file, bypassing APT's repositories entirely. Useful for software distributed as a standalone download.

10. **pip / npm install** — language-specific package managers for Python and Node.js respectively. Worth knowing they exist alongside the system-level package managers, since they operate in a completely separate space.
