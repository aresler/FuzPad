<h1 align="center">📙FuzPad!</h1>

<p align="center">
    <em>FuzPad is a minimalistic note management solution. Powered by ⚡<a href="https://github.com/junegunn/fzf">junegunn/fzf</a></em>⚡
</p>

<p align="center">
 <img src="https://i.imgur.com/5WXsOH1.png" alt="Sample Image" width="350"/>
 <img src="https://i.imgur.com/lkyY8Fe.png" alt="Sample Image" width="350"/>
 <img src="https://i.imgur.com/NMbPXN7.png" alt="Sample Image" width="350"/>
 <img src="https://i.imgur.com/5IljHKS.png" alt="Sample Image" width="350"/>
</p>

[![Star History Chart](https://api.star-history.com/svg?repos=JianZcar/FuzPad&type=Timeline)](https://star-history.com/#JianZcar/FuzPad&Timeline)

## Features
- **New**: Create a new note with the current date and time as the filename.
- **Open**: Open an existing note.
- **Search**: Search within notes for specific content.
- **Delete**: Delete selected notes.
- **Version control**: automatically commits changes to your notes.

## Planned Features
- **Tags**: tagging system
- **Make an installer**: use brew for packaging
- **CLI**: create a cli that allows piping, etc.

## Goals

- Provide a straightforward and minimalistic note management solution using a Bash script.
- Ensure ease of use with intuitive commands and interface.

## Requirements

- Bash
- [fzf](https://github.com/junegunn/fzf) (fuzzy finder)
- [bat](https://github.com/sharkdp/bat) (for enhanced preview)
- Your preferred text editor (default is `nano`)

## Usage

1. Clone the repository:

```sh
git clone https://github.com/JianZcar/notes-bash.git
cd notes-bash
```

2. Make the script executable:

```sh
chmod +x bin/notes
```

3. Run the script:

```sh
./bin/notes
```

## Configuration

- **Default Directory**: Change the default directory for notes by modifying the `FUZPAD_DIR` variable in the script or by setting it in your `~/.bashrc` file:
  ```sh
  export FUZPAD_DIR="$HOME/Documents/.notes"
  ```

- **Text Editor**: Change the text editor by modifying the `EDITOR` variable in the script or by setting it in your `~/.bashrc` file:
  ```sh
  export EDITOR="nano"
  ```

- **Text Format**: Change the text format by modifying the `TEXT_FORMAT` variable in the script or by setting it in your `~/.bashrc` file:
  ```sh
  export FUZPAD_TEXT_FORMAT="txt"
  ```

- **Date Time Format**: Change the date and time format used for note filenames by modifying the `DATE_TIME_FORMAT` variable in the script or by setting it in your `~/.bashrc` file:
  ```sh
  export FUZPAD_DATE_TIME_FORMAT="%Y-%m-%d-%H-%M-%S"
  ```

- **BAT Theme**: Change the theme used by `bat` for previewing notes by modifying the `BAT_THEME` variable in the script or by setting it in your `~/.bashrc` file:
  ```sh
  export FUZPAD_BAT_THEME="OneHalfLight"
  ```

- **Reverse List**: Set to `true` to reverse the order of the list when opening or deleting notes by modifying the `REVERSE_LIST` variable in the script or by setting it in your `~/.bashrc` file:
  ```sh
  export FUZPAD_REVERSE_LIST="false"
  ```

- **Sort Format**: Change the sorting format for listing notes (`T@` for creation date, `Y` for modified date) by modifying the `SORT_FORMAT` variable in the script or by setting it in your `~/.bashrc` file:
  ```sh
  export FUZPAD_SORT_FORMAT="T@"
  ```

- **Preview Size**: Change the size of the preview window for `fzf` by modifying the `PREVIEW_SIZE` variable in the script or by setting it in your `~/.bashrc` file:
  ```sh
  export FUZPAD_PREVIEW_SIZE="70%"
  ```

- **Start Line Search Preview**: Set the starting line number for the search preview by modifying the `START_LINE_SEARCH_PREVIEW` variable in the script or by setting it in your `~/.bashrc` file:
  ```sh
  export FUZPAD_START_LINE_SEARCH_PREVIEW="5"
  ```

- **End Line Search Preview**: Set the ending line number for the search preview by modifying the `END_LINE_SEARCH_PREVIEW` variable in the script or by setting it in your `~/.bashrc` file:
  ```sh
  export FUZPAD_END_LINE_SEARCH_PREVIEW="9999"
  ```

After adding the necessary variables to your `~/.bashrc` file, remember to source it to apply the changes:
```sh
source ~/.bashrc
```

## Contributing

Feel free to fork the repository and submit pull requests. Contributions are welcome!

## License

This project is licensed under the terms of the GNU General Public License v3.0. For more details, see the [LICENSE](LICENSE) file in the repository.
