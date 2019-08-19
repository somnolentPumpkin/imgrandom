# Random Image Grabber

A command line tool that grabs images of random sizes from [Lorem Picsum](https://picsum.photos).

## Requirements
- ```wget``` must be installed and accessible from your terminal.

## Usage
The only argument is the number of images you want to grab (default: 10).

```
./random_image_grabber.sh <amount>
```

**Example:**
```
./random_image_grabber.sh 10
```

The above example will grab 10 images of random widths and heights.

## Install + Run
1. Download the ```random_image_grabber.sh``` file.
2. Run ```chmod +x random_image_grabber.sh```.
3. Run ```./random_image_grabber.sh```

### Why do I have less images than I specified?
If something goes wrong during the download, wget saves an empty file. When the script is done running, it cleans up the empty files. If you have less images than expected, one or more images didn't download and was cleaned up.
