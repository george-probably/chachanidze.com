# Chachanidze.com
This is a repo for the [chachanidze.com](https://chachanidze.com) Weblog. Please note that you may see posts in here that aren't quite ready for prime-time! I am trusting you to be considerate of the work-in-progress.

## Layout

| Folder            | Contents                                                                                                                          |
|-------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| Images            | Occasionally posts with need hosted images instead of something from Unsplash. In those rare situations, they are hosted here.    |
| Weblog            | This is where all of the files that [weblog.lol](https://weblog.lol) can actually see reside, within subfolders listed below.     |
| .../Configuration | These configuration files are required for [weblog.lol](https://weblog.lol), and feature the main template and a config file.     |
| .../Pages         | Any page that isn't a blog post belongs in here, they tend to also require their own template.                                    |
| .../Posts         | This folder contains the Markdown files for each blog post, they are sub-divided into `Year/Month`.                               |
| .../Templates     | Though the main template is housed in `/Configuration`, the secondary templates for non-post pages are hosted within this folder. |
| .github/Workflows | This contains the main.yml file needed to kick off the task of updated the weblog whenever this repo is changed.                  |