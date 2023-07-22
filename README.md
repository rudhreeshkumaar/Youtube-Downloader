# YouTube Downloader

This Python script allows you to download YouTube videos by providing the video link as a command-line argument. The script utilizes the `pytube` library to fetch video details and download the video at the highest available resolution.

## Prerequisites

Before running the script, make sure you have the `pytube` library installed. You can install it using `pip`:

```
pip install pytube
```

## Usage

1. Save the script in a Python file, e.g., `youtube_downloader.py`.
2. Open your command-line or terminal.
3. Execute the script with the YouTube video link as a command-line argument.

```
python youtube_downloader.py <youtube_video_link>
```

Replace `<youtube_video_link>` with the actual YouTube video link you want to download.

## Script Description

1. The script imports the `YouTube` class from the `pytube` library.
2. It accepts a YouTube video link as a command-line argument using `argv[1]`.
3. The script creates a `YouTube` object `yt` with the provided video link.
4. It prints the title and view count of the YouTube video using `yt.title` and `yt.views` respectively.
5. The script gets the highest resolution stream using `yt.streams.get_highest_resolution()`.
6. The video is downloaded to the specified folder (`./YTfolder`) using `yd.download('./YTfolder')`.

## Note

- Make sure to replace `'./YTfolder'` with the desired folder path where you want to save the downloaded video.
- Ensure that the `pytube` library is correctly installed and compatible with your Python environment.
- Respect copyright and usage policies when downloading YouTube videos.

Enjoy using this simple YouTube video downloader to save your favorite videos locally!
