## Cursor & Icon Collection

A collection of custom cursors and icons, compatible with both **X11** and **Wayland** desktop environments.

## Installation Instructions

### Clone the Repository
First, clone this repository to your local machine:
```bash
git clone https://github.com/harilvfs/icons
```

### Change to the Cloned Directory
Navigate into the directory that contains the cursors and icons:
```bash
cd icons/
```

### Install the Cursors & Icons

You can install the cursors and icons either system-wide or for a specific user.

#### Option 1: System-Wide Installation
Move all the cursors and icons to the system's shared icon directory:
```bash
sudo mv * /usr/share/icons/
```

#### Option 2: User-Specific Installation
Alternatively, you can install the cursors and icons for a single user by creating a custom directory in your home configuration:
```bash
mkdir -p ~/.config/icons
mv * ~/.config/icons/
```

If the `~/.config/icons/` directory doesn't exist, the above command will create it.

## Applying the Cursors & Icons

After installing the icons and cursors, you need to apply them. The steps differ depending on whether you're using **X11** or **Wayland**.

### For X11

To apply icons and cursors on an **X11**-based system, use **lxappearance**:

Install **lxappearance** if you haven’t already:
   ```bash
   sudo pacman -S lxappearance
   ```

Launch **lxappearance**:
   ```bash
   lxappearance
   ```

In **lxappearance**, you can select and apply the newly installed icons and cursors under the "Icon Theme" and "Cursor Theme" sections.

### For Wayland

On **Wayland**, you can use **nwg-look** for GTK and **Kvantum** for Qt-based applications.

#### Install the required packages for Wayland:

- **nwg-look** for GTK themes:
  ```bash
  sudo pacman -S nwg-look
  ```

- **kvantum-qt5** (or **kvantum-qt6**) for Qt themes:
  ```bash
  sudo pacman -S kvantum-qt5
  ```
  *For Qt6 applications:*
  ```bash
  sudo pacman -S kvantum-qt6
  ```

#### Applying the themes:

**nwg-look**: To apply the icons and cursors for GTK applications:
   ```bash
   nwg-look
   ```
   Select your icons and cursors from the relevant sections and apply.

**Kvantum Manager**: To apply the theme for Qt applications:
   ```bash
   kvantummanager
   ```
   Select and apply your icons and cursors under the "Change/Delete Theme" tab.

## License

This cursor and icon collection is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.

---

MIT License

