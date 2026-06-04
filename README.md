# Sofle

![Sofle键位图](keymap-drawer/eyelash_sofle.svg)

## Host OS setup (EurKEY layout)

This firmware is **layout-dependent**: the keyboard sends US-position key codes,
and the operating system decides which character each one produces. This keymap
is built for the [**EurKEY**](https://eurkey.steffen.bruentjen.eu) layout — a
US-QWERTY base with European letters on the AltGr layer — which is published
identically for Windows, macOS, and Linux. Set EurKEY as the active layout on
every machine and the keyboard behaves the same everywhere (including `ä ö ü`
via AltGr). Without it active, symbols and accented letters will be wrong.

You change the **software input layout**, not the physical keyboard hardware
setting.

### Windows

1. Download the EurKEY installer from <https://eurkey.steffen.bruentjen.eu> and run it.
2. Sign out and back in (or reboot) so Windows registers the layout.
3. **Settings → Time & language → Language & region →** your language **→ ⋯ →
   Language options → Add a keyboard → EurKEY**.
4. Switch to it with **Win + Space** (or the taskbar language indicator).
5. *(Optional)* Remove the other keyboards under that language so EurKEY is the
   only one and can't be switched away by accident.

### macOS

1. Download the macOS package from <https://eurkey.steffen.bruentjen.eu> and unzip it.
2. Copy **`EurKEY.bundle`** into **`~/Library/Keyboard Layouts/`** (current user)
   or **`/Library/Keyboard Layouts/`** (all users).
3. Log out and back in (or reboot) so macOS picks up the new layout.
4. **System Settings → Keyboard → Text Input → Input Sources → Edit → `+` →**
   find **EurKEY** (listed under *Others* / *English*) **→ Add**.
5. Select it from the input menu in the menu bar (or **Ctrl + Space**).
6. *(Recommended)* Remove other input sources so EurKEY stays active.

> Note: macOS gives both Alt/Option keys the AltGr role, so `ä`/`ö`/`ü` (AltGr+a/o/u)
> work with either thumb modifier.

### Linux

EurKEY ships with `xkeyboard-config`, so no download is needed:

- **GNOME/KDE:** add the input source **“EurKEY”** (English layout, EurKEY variant).
- **X11/CLI:** `setxkbmap eu`

### Verifying

After flashing and selecting EurKEY, tap the symbol layer and confirm a few keys
(`@ # { } [ ] \ ~ ^`) and the umlauts (`ä ö ü`). They should match the keymap
diagram above on **every** OS. If a whole class of symbols is off, the active OS
layout is almost certainly not EurKEY.

## Seller info

For 3D printed model files or any issues and malfunctions with the keyboard, please contact [380465425@qq.com](mailto:380465425@qq.com)