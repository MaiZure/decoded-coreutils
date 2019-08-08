# Decoded-GNU-Coreutils comment repo

This repo contains the comments used to generate the line-by-line walkthroughs for the [Decoded-GNU-Coreutils project](http://www.maizure.org/projects/decoded-gnu-coreutils). 

The .comment files are skeletons to fill in over time. These .comment files are combined with the source from my mirror of the v8.3 source and generated markup on the website.

For example: The [whoami](https://github.com/MaiZure/coreutils-8.3/blob/master/src/whoami.c) source is combined with the [whoami.comments](https://github.com/MaiZure/decoded-coreutils/blob/master/comments/whoami.comment) file and the [resulting walkthrough](http://www.maizure.org/projects/decoded-gnu-coreutils/whoami_walkthrough.html) is generated on my website via some server-side scripting magic. (magic not included in this repo) 

As of August 2019, only 'whoami' has any useful contributions. All others are utilities are placeholders that are generated, but mostly useless. Such as: 
[tee](http://www.maizure.org/projects/decoded-gnu-coreutils/tee_walkthrough.html),
[timeout](http://www.maizure.org/projects/decoded-gnu-coreutils/timeout_walkthrough.html)

## Files
In addition to .comment files there are three other special files tha contain common elements used among all utilities:
```bash
!syscalls
!includes
!common
```
Entries in these files will apply to occurrances across all utilties. However, these can be overrided by adding the line manually to the specific utility

## Usage
Look at the .comment files to see how they work. For now, the 'whoami' comments and results are the model to use. In general, a line number and a comment on a single line.

The only markup current supported is a double space forces a new line. I may make this more complicated as time goes by...or maybe not. KISS

## Contributions
Feel free to contribute although I admit this is a huge workload and quite boring. I'll knock it out myself over the long haul

NOTE: Updating this repo does not immediately for the website to update. I have to cast the spells manually for now.
