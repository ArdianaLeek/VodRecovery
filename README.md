# VodRecovery
* The purpose of this script is to obtain videos or clips that are either marked as "sub-only" or have been deleted on Twitch. 

# About
* Developed by: Shishkebaboo (formerly ItIckeYd, the original developer who is back to work on the project after a hiatus)
* Initial release: May 3rd, 2022
* The script leverages logic from the [TwitchRecover](https://github.com/TwitchRecover/TwitchRecover) repository developed by [Daylam Tayari](https://github.com/daylamtayari)

# Features
* Supports both manual and website vod recovery
* Can recover vods individually or in bulk using a CSV downloaded from [Sullygnome](https://sullygnome.com/)
* Can recover clips manually or in bulk using a CSV from [Sullygnome](https://sullygnome.com/)
* Supports downloading M3U8 links/files, with the ability to specify start/end timestamps for trimmed vods using [FFmpeg](https://ffmpeg.org/download.html)
* Compatible with [TwitchTracker](https://twitchtracker.com/), [Sullygnome](https://sullygnome.com/), and [Streamscharts](https://streamscharts.com/)
* Uses UTC timezone as default for recovering vods
* Notifies if vod is older than 60 days (due to Twitch's deletion process)

# Installation
* Download/install - [Python](https://www.python.org/downloads/)
* Clone the repository
* Navigate to the cloned directory
* Install required packages with `pip install -r requirements.txt` (run in terminal)
* If you make changes to installed packages locally, you can overwrite the requirements.txt file with `pipreqs <path_of_project> --force`
* Run the script

### Expected Script Output

```
WELCOME TO VOD RECOVERY

1) Recover Vod
2) Recover Clips
3) Unmute an M3U8 file
4) Check M3U8 Segments
5) Generate M3U8 file (ONLY includes valid segments)
6) Download M3U8 (.MP4 extension)
7) Exit

Please choose an option:
```

### Expected FFmpeg Ouput
* Run the `ffmpeg` command in Command Prompt

![ffmpeg_preview](https://user-images.githubusercontent.com/118132878/216841020-617b9807-3a4c-4f03-856e-854d91306880.png)

# Configuration File
* The configuration file can be used to limit the amount of user input when using the script. The following options are among the most popular to change for users:
 1. ```UNMUTE_VOD```
 2. ```CHECK_SEGMENTS```
 3. ```DOWNLOAD_CLIPS```
 4. ```REMOVE_LOG_FILE```
 5. ```DEFAULT_DIRECTORY```
 6. ```DOWNLOAD_DIRECTORY```

### Default Configuration
![config_file_vodrecover](https://user-images.githubusercontent.com/118132878/220527660-54a2f47c-20cf-4c2d-b4d1-7c9866835ad4.png)


# Optional IDEs
* [PyCharm Community Edition](https://www.jetbrains.com/pycharm/download/) (recommended)
* [Visual Studio Code](https://code.visualstudio.com/download)

# Additional Notes
* Provide at least one example when creating an issue
* If the script returns no results, try vods from other streamers. If the other vods return results, it is likely that the original vods don't exist.

# Support the Project
* Donations are appreciated but not expected - [PayPal](https://paypal.me/VodRecovery)

# Latest Release
* [Stable Release - 1.0.0.8](https://github.com/Shishkebaboo/VodRecovery/releases/tag/vodrecovery-1.0.0.8)
* For the most updated code, clone the main branch of the repository.

