# python-torrent-tree

This is a Python script that parses a torrent file and extracts file data from it. It can build a tree-like structure of the files and directories present in the torrent.

## Requirements

- Python 3.x
- bencodepy (a library to parse bencoded data) - You can install it using `pip install bencode.py`.

## Usage

1. Place the `test.torrent` file in the same directory as the script.

2. Run the script `torrent_parser.py`.

3. The script will read the `test.torrent` file, extract the file data, and build a tree-like structure representing the files and directories.

4. The resulting tree structure will be printed in JSON format.

## Function Documentation

### parse_torrent(torrent_file_path: str) -> list[dict]

Parse the torrent file and extract the file data.

Parameters:
- `torrent_file_path` (str): The path to the torrent file.

Returns:
- `list[dict]`: A list of dictionaries, each containing the 'path' and 'length' of a file.

### build_path_tree(file_data_list: list[dict]) -> dict

Build the tree-like structure out of the file data.

Parameters:
- `file_data_list` (list[dict]): A list of dictionaries, each containing the 'path' and 'length' of a file.

Returns:
- `dict`: A dictionary representing the tree-like structure of the files and directories, with the file lengths as values.

