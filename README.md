# clipimage

A simple CLI tool to save clipboard images to files.

## Installation

### From npm registry (when published)

```bash
npm install -g clipimage
```

### From local directory (for development)

For Windows PowerShell or WSL:

```bash
# Navigate to the project directory
cd /path/to/ClipImageToFile

# Install globally from current directory
npm install -g .
```

After installation, you can use `clipimage` command from anywhere.

## Usage

```bash
# Save clipboard image with default name (clipboard-image.png)
clipimage

# Save with custom filename
clipimage -o myimage.png

# Save in different format
clipimage -o myimage -f jpg

# Show help
clipimage --help
```

## Options

- `-o, --output`: Output file path (default: clipboard-image.png)
- `-f, --format`: Output format - png, jpg, jpeg, bmp (default: png)
- `-h, --help`: Show help

## Supported Platforms

- Windows
- macOS
- Linux (requires xclip)

## Linux Requirements

On Linux, you need to have `xclip` installed:

```bash
sudo apt-get install xclip  # Ubuntu/Debian
sudo yum install xclip      # RHEL/CentOS
```

## License

MIT