# SETVRename
Renames TV show files to Season/Episode format.

## Preface

I created this tool to help assist me in archiving my TV shows from DVD and Blu-Ray. To name my files properly, I decided to use [theRenamer](http://www.therenamer.com); however, it requires the files to be in the following format:

```
Show
    Season 1
        S01E01.mp4
        S01E02.mp4
        S01E03.mp4
        S01E04.mp4
        S01E05.mp4
        S01E06.mp4
        S01E07.mp4
        S01E08.mp4
```

But after archiving the files, I was always left with something like this:

```
Show
    Season 1
        title00.mp4
        title01.mp4
        title02.mp4
        title03.mp4
        title04.mp4
        title05.mp4
        title06.mp4
        title07.mp4
```

Which meant I had to manually go update the filename of each show one by one - so, I created this tool.

## Installation

1. Ensure you have the proper .NET redistributables installed on your PC
2. download this repository to desired folder


## Usage

1. Place your video files in order within a folder titled `Season X` (*X* being the season that this group of episodes belong to).
2. Run `SETVRename.exe "/path/to/Season X"`
  * The program then  runs through all the files in `/path/to/Season X`, and renames the files to `SXEY`, where `X` is the season number in the containing folder name, and Y is it's position in alphabetical order

