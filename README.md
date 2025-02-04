# Discord Gif Splitter

Fun project I made for fun.

This is basically a wrapper around FFmpeg, but easier to use.

## Download

#### You must have FFmpeg installed for this to work. The [FAQ](#FAQ) section has more information.

#### If you're having trouble installing FFmpeg, download the `_with_ffmpeg.zip` version

[You can download the program here](https://github.com/Malpp/DiscordGifSplitter/releases)

## Demo

![Demo](DemoFiles/Demo.gif)
![Demo Results](DemoFiles/Demo_Results.png)
![Demo Discord](DemoFiles/Demo_Discord.gif)

## Usage

Step by step guide
1. Drag the image into the program
2. Adjust the splitting grid to your liking
3. Give it a name
4. Click Create
5. Find a folder where the Gifs can be stored
6. Open the `.txt` file that it created and copy paste in discord to see your new wall of emotes

## <a name="FAQ"></a>FAQ

### Q: I get the `FFmpeg not found. Please make sure FFmpeg is in PATH.` message when creating my images
A: You must have FFmpeg installed on your computer for this program to work. To install it correctly, here is a guide: https://github.com/adaptlearning/adapt_authoring/wiki/Installing-FFmpeg

#### If the download link is not working, download it from [here](https://ffmpeg.zeranoe.com/builds/win64/static/ffmpeg-20180502-e07b191-win64-static.zip)

To be sure you have it installed on your system, open a `CMD` window and type `ffmpeg -version` to validate it is working.

#### If the FFmpeg install still doesn'work work, you can try the following

1. Download this [zip](https://ffmpeg.zeranoe.com/builds/win64/static/ffmpeg-20180502-e07b191-win64-static.zip)
2. Go in the `bin` folder
3. Copy `ffmpeg.exe`
4. Paste it where `DiscordGifSplitter.exe` is located

### Q: Sometimes I see my image being repeated? Is this normal?
A: Yes, this is due to the grid being outside of the image. Currently the best situation is to crop the image a bit.

### Q: My Frames are being stacked when i use a transparent gifs! How do i fix that?
A: This is fixed in the Release https://github.com/philipo30/DiscordGifSplitter/releases/tag/v1.2.2 . The problem was caused by FFmpeg.

### Q: Why do the emojis dont get uploaded as animated emojis in Discord?
A: This happens due to Discord limiting emoji sizes to 256 KB. To fix this go to https://ezgif.com/optimize and upload the emoji that is too big. Next set the optimization method to lossy Gif and compression level to 5, as it should be enough. If not increase a little until the size is below 256 KB.
![compressinggif](DemoFiles/compressinggif.png)
