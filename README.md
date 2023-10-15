# resize_images.sh
Resizes all images in the specified directory incl. subdirectories

## Features

- Progress bar
- Processing summary
- JSON output
- Quiet mode
- Small automatic image image enhancements (-filter Lanczos2Sharp -unsharp 1.5x1+0.7+0.02 -brightness-contrast 1x5)
- Supported file formats: jpg, png, tif, heif, heic, webp

## Screenshot

![Demo Screenshot]([https://via.placeholder.com/468x300?text=App+Screenshot+Here](https://github.com/whollaus/resize_images.sh/blob/main/SCR-20231015-oqvq.png))

## Options:

 		-h, --help           Display this help message.
 		-s, --src            Source directory containing the original images.
 		-d, --dest           Destination directory for the resized images.
 		-q, --quiet          Run in quiet mode (suppress all output).
 		-m, --max-dimension  Set maximum dimension for the longer side of the image.
 		-q, --quality        Set quality for the resized images (1-100).
 		-j, --json        	 Display the summary in json format.

## Dependencies:

--- Attention: Developed and tested only under MacOS ---

- ImageMagick (convert command)
```bash
brew install imagemagick
```
- bc
- du
- touch

## Installation:

- Download the resize_images.sh Script
- Make the script executable:
```bash
  chmod +x resize_images.sh
```

## Usage

```bash
resize_images.sh -s ./originals -d ./resized -m 800 -q 80
```

## Roadmap

Nothing planned

## License:

[MIT](https://choosealicense.com/licenses/mit/)

## Authors

- [@whollaus](https://github.com/whollaus) form [HOLLAUS-IT](https://hollaus-it.at/)

## Versions:

- 2023/10/15 : whollaus : First release
