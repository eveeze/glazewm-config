# Glazewm Cheatsheet

Below are tables summarizing the keybindings and commands from your configuration.

---

## Focus Navigation & Window Movement

| **Keybinding(s)**                 | **Command**               | **Description**              |
| --------------------------------- | ------------------------- | ---------------------------- |
| `alt+h` / `alt+left`              | `focus --direction left`  | Focus window to the left     |
| `alt+l` / `alt+right`             | `focus --direction right` | Focus window to the right    |
| `alt+k` / `alt+up`                | `focus --direction up`    | Focus window above           |
| `alt+j` / `alt+down`              | `focus --direction down`  | Focus window below           |
| `alt+shift+h` / `alt+shift+left`  | `move --direction left`   | Move focused window left     |
| `alt+shift+l` / `alt+shift+right` | `move --direction right`  | Move focused window right    |
| `alt+shift+k` / `alt+shift+up`    | `move --direction up`     | Move focused window upward   |
| `alt+shift+j` / `alt+shift+down`  | `move --direction down`   | Move focused window downward |

---

## Resizing Commands

| **Keybinding(s)** | **Command**                            | **Description**                                                        |
| ----------------- | -------------------------------------- | ---------------------------------------------------------------------- |
| `alt+u`           | `resize --width -2%`                   | Decrease window width                                                  |
| `alt+p`           | `resize --width +2%`                   | Increase window width                                                  |
| `alt+o`           | `resize --height +2%`                  | Increase window height                                                 |
| `alt+i`           | `resize --height -2%`                  | Decrease window height                                                 |
| `alt+r`           | `wm-enable-binding-mode --name resize` | Enter resize mode (use arrow keys or HJKL, exit with `escape`/`enter`) |

---

## Tiling, Floating & Fullscreen Toggles

| **Keybinding(s)** | **Command**                  | **Description**                                       |
| ----------------- | ---------------------------- | ----------------------------------------------------- |
| `alt+v`           | `toggle-tiling-direction`    | Change tiling direction (new windows insertion point) |
| `alt+shift+space` | `toggle-floating --centered` | Toggle floating mode (centered by default)            |
| `alt+t`           | `toggle-tiling`              | Switch focused window to tiling mode                  |
| `alt+f`           | `toggle-fullscreen`          | Toggle fullscreen mode                                |
| `alt+m`           | `toggle-minimized`           | Minimize the focused window                           |

---

## Window & WM Management

| **Keybinding(s)** | **Command**                           | **Description**                                                  |
| ----------------- | ------------------------------------- | ---------------------------------------------------------------- |
| `alt+shift+q`     | `close`                               | Close the focused window                                         |
| `alt+shift+e`     | `wm-exit`                             | Safely exit GlazeWM                                              |
| `alt+shift+r`     | `wm-reload-config`                    | Reload the configuration file                                    |
| `alt+shift+w`     | `wm-redraw`                           | Redraw all windows                                               |
| `alt+shift+p`     | `wm-enable-binding-mode --name pause` | Enable pause mode (all other keybindings disabled until toggled) |

---

## Application Launchers

| **Keybinding(s)** | **Command**                                     | **Description**           |
| ----------------- | ----------------------------------------------- | ------------------------- |
| `alt+enter`       | `shell-exec wezterm-gui`                        | Launch terminal (Wezterm) |
| `alt+c`           | `shell-exec chrome --profile-directory=Default` | Launch Chrome             |

---

## Workspace Management

| **Keybinding(s)**              | **Command**                                                    | **Description**                                              |
| ------------------------------ | -------------------------------------------------------------- | ------------------------------------------------------------ |
| `alt+s`                        | `focus --next-workspace`                                       | Focus the next workspace                                     |
| `alt+a`                        | `focus --prev-workspace`                                       | Focus the previous workspace                                 |
| `alt+d`                        | `focus --recent-workspace`                                     | Focus the most recently used workspace                       |
| `alt+1` to `alt+9`             | `focus --workspace <number>`                                   | Directly focus workspace `<number>`                          |
| `alt+shift+1` to `alt+shift+9` | `move --workspace <number>`, then `focus --workspace <number>` | Move focused window to workspace `<number>` and switch to it |
| `alt+shift+a`                  | `move-workspace --direction left`                              | Move current workspace to the left (across monitors)         |
| `alt+shift+f`                  | `move-workspace --direction right`                             | Move current workspace to the right                          |
| `alt+shift+d`                  | `move-workspace --direction up`                                | Move current workspace upward                                |
| `alt+shift+s`                  | `move-workspace --direction down`                              | Move current workspace downward                              |
