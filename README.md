# Hyprkeys

A simple, and relatively fast application that returns your Hyprland keys.

*No, not just keybinds. We now return config sections as well*


> ⚠️ Hyprkeys is currently in early development and is not ready for use. Not like it can
break anything, but you will have wasted your time.

In case you still want to use it, instructions are below:

**(Looking for testers and contributors, Go is not a language I often work with.)**

## Installation & Usage

1. Download Go. You can find it [here](https://golang.org/dl/)
2. Clone this repository with `git clone https://github.com/notashelf/hyprkeys`
3. Install the application with `make build` then `sudo make install`
5. You can run the application with `hyprland`

## Project Roadmap

- [x] Format keybinds better, maybe with a proper table
  - [x]  Remove the `+` in the keybinds that don't have modifiers
  - [x]  Add an extra column to mouse keybinds to match table titles
- [x] Optionally (--variables) parse variables and replace them with their actual value
- [x] Account for bind flags, that may be passed in any random order
  - [x] Figure out a regex to match the flags
    - [x] Figure out why the regex doesn't work
- [x] Account for line comments in rows
- [x] Break code into multiple files
    - [x] move command line parsing to a separate file
- [ ] Command line options
  - [ ] Sort output by dispatcher
  - [x] Account for multiple arguments being passed at once
- [ ] Somehow account for keybinds can be set dynamically? (I don't know how to do this)
  - [ ] Add instructions for a pipe to `hyprkeys` to get the keybinds from
- [ ] Convert i3/sway keybinds to Hyprland keybinds with `--convert`
  - [ ] Possibly more wayland compositors, sway is enough for now.
- [x] Get more than just keybinds, try and get all config options seperated by section
  - [x] Config sections
  - [x] Autostarted applications
  - [x] Keywords from inside `hyprland.conf`
- [ ] **Packaging for various Linux distros**
  - [ ] Nix (WIP)
    - [ ] Flake
    - [ ] Legacy nixpkgs package
  - [ ] Arch (looking for maintainers)
  - [ ] Fedora (looking for maintainers)

https://user-images.githubusercontent.com/86447830/211897915-778e9b24-061d-4d97-bc5e-444224610566.mp4

Rofi script using hyprctl:

![OrCEzxZ - Imgur](https://user-images.githubusercontent.com/86447830/211898056-3bdb2f11-f7f5-4854-871f-4eabaa5b898f.png)

## Example Outputs (as of 11 JAN 2023)

**[MARKDOWN](test/out.md)**

**[JSON](test/out.json)**

**[RAW](test/out.txt)**

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contributing

If you want to contribute, feel free to open a pull request. I'll try to review it as soon as possible.
