# Zebar Widget - Fucking Test

This is a custom widget for `zebar`status bar. It provides a frosted glass bar with several information modules.

## Features

*   **System Info:** CPU, Memory, and Battery status.
*   **Audio Control:** View and control system volume with a clickable slider.
*   **Media Player and Visualizer:** Displays the currently playing song and visualizer with playback controls.
*   **Weather:** Shows the current temperature and a weather icon.
*   **Customizable Appearance:** Translucent background with a blur effect and a random background image from Unsplash.

## Prerequisites

1. [Zebar](https://github.com/glzr-io/zebar)

## Setup Instructions

1.  Get the project and widget
    *   Open zbar from taskbar tray
    *   Create a custom project named "fucking_zebar" with custom widget named "fucking_test"
    *   Open the project in code editor from `C:\Users\<YourUsername>\.glzr\zebar\fucking_zebar\`
    *   copy the `zpack.json` in project directory and `index.html` and `styles.css` in widget from this project into the new folder. 
    * Copy the settings.json in the zbar folder
    * Your file structure should look like this:
        ```
        C:\Users\<YourUsername>\.glzr\
        └── zebar\
            └── settings.json
            └── fucking_zebar
                └── zpack.json
                └── fucking_test\
                    ├── index.html
                    └── styles.css
        ```


2. Make a task scheduler basic task for zebar launch on startup:

* Open Task Scheduler:

* Create Basic Task:

* Name and Description: Anything

* Click "Next".

* Add Trigger: Choose "When I log on" (Recommended for most users): This is usually best for applications like Zebar, as it starts after your user profile is loaded.
<!-- 
(note to self - actually next time try syste startup action trigger)
"When the computer starts": This runs the task very early in the boot process, even before anyone logs in. This might be useful if Zebar needs to be active system-wide from the absolute start, but can sometimes cause issues if it relies on user-specific resources or network connections that aren't ready yet. -->

* Click "Next".

* Add Action:
    - Select "Start a program".

    - Click "Next".

    - Add Program/Script, Click "Browse..." and navigate to your zebar.exe file. Select it. Example path: "C:\Program Files\Zebar\zebar.exe" (adjust if yours is different).

    - Add arguments (optional): leave empty.

    - Start in (optional): leave empty.

* Click "Next".

* Click "Finish".

* Make sure it says User on "select user group" otherwise make it say that.

3. fucking_reboot

* Advanced Settings:

![img](https://github.com/ParamAhuja/zebar_configs/blob/main/resources/image.png)
![img](https://github.com/ParamAhuja/zebar_configs/blob/main/resources/image2.png)

