# Workspace Indicator - Fork

Fork of GNOME's `workspace-indicator` extension with a separate UUID and settings schema so it can coexist with the stock extension.

This copy was created from the locally installed `Workspace Indicator` extension and keeps the upstream behavior unchanged.

## Install

Install it into your local GNOME Shell extensions directory:

```bash
cp -a . ~/.local/share/gnome-shell/extensions/workspace-indicator-fork@elidon555.github.com
cd ~/.local/share/gnome-shell/extensions/workspace-indicator-fork@elidon555.github.com
glib-compile-schemas schemas
gnome-extensions enable workspace-indicator-fork@elidon555.github.com
```

If GNOME Shell does not pick it up immediately, reload the shell or log out and back in.

## After Install

- The forked extension UUID is `workspace-indicator-fork@elidon555.github.com`.
- The stock extension can stay installed, but if you do not want two indicators in the panel, disable the stock one.
- If you change the schema XML later, run `glib-compile-schemas schemas` again.
- A real copied directory is safer than a symlink here, because GNOME Shell may ignore symlinked extension directories.
