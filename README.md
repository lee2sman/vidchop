# vidchop

A simple command line video-editing program, built on ffmpeg.

ffmpeg is an incredible swiss army knife of a toolkit for video editing. Unfortunately, its expansive nature means it's not very discoverable and one must often perform a web search and then try out various options until the correct result is achieved. vidchop is intended to simplify the usage of ffmpeg with clean, concise syntax.

This is an early prototype status. Polite bug reports may be considered.

```
usage: vidchop <option> <input-file> [<output-file>]

   --help    | -h  : prints this help
   --output  | -o  : output file. (default output.mp4)
INFO:
   --info    | -i
   --length  | -l  : get length in HH:mm:ss.ms
   --seconds | -s  : get length in seconds
PROCESS:
    --reduce | -r  : fast compress input file
    --trim   | -t  : cut from hh:mm:ss to hh:mm:ss
    --combine| -c  : sequentially combine videos input list file

For combining videos, listfile must be formatted:
file 'file1.mp4'
file 'file2.mp4'
..etc..
```
