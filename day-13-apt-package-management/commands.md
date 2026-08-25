#  Day 13: APT Package Management (Debian/Ubuntu)

1. **apt update** — refreshes the local index of available packages from the configured repositories. This doesn't install or upgrade anything itself — it just makes sure APT knows what's currently available.

2. **apt upgrade** — installs newer versions of already-installed packages, based on the index `apt update` just refreshed. It won't remove any existing packages to do so.

3. **apt full-upgrade** — like `apt upgrade`, but willing to remove packages if that's what's needed to complete an upgrade. More thorough, but slightly riskier if you care about exactly what stays installed.

4. **apt install** — installs a new package by name, along with any dependencies it needs.

5. **apt remove** — uninstalls a package but leaves its configuration files behind, in case you want to reinstall it later with the same settings.

6. **apt purge** — uninstalls a package and its configuration files together, for a genuinely clean removal.

7. **apt autoremove** — clears out packages that were installed as dependencies but are no longer needed by anything currently installed. Good general housekeeping after removing software.

8. **apt search** — searches package names and descriptions for a keyword, which is how I'd find the right package name before installing anything.

9. **apt show** — displays detailed information about a specific package — version, size, dependencies, description — without installing it.

10. **dpkg -l / dpkg -L** — `dpkg -l` lists every package currently installed on the system; `dpkg -L` lists every file belonging to one specific package.
