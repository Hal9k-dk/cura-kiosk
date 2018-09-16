# Cura configuration @ hal9k

Configuration files under `.config/cura` and `.local/share/cura` are kept in
Git repositories. When Cura is launched, all untracked files and deleted and
changes are discarded. The desktop icon runs the `run-cura` which runs
`config-reset` before launching Cura.

To make persisent configuration changes, you need to commit these changes
before running Cura again. Run the `config-commit` script to do this. Changes
can be inspected using the `config-status` and `config-diff` scripts, but be
wary that Cura will jumble the configuration files. It seems that the options
are written in random order each time.
