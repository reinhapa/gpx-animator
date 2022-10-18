# GPX Animator
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-27-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

## Introduction

GPX Animator generates a top-down view map video from one or more GPX files generated by most standard GPS tracking devices.

GPX Animator has a graphical user interface that works on most operating systems, but works with a pure command-line interface as well.

More information and downloadable executables can be found at https://gpx-animator.app.

## Basic usage

```
# help
java -jar gpx-animator-x.y.z-all.jar --help

# create movie with default settings
java -jar gpx-animator-x.y.z-all.jar --input track.gpx
```
(where `x.y.z` refers to the version of the jar you built or downloaded)

## Advanced command line example

This example takes GPX file `input.gpx` as input, uses Google Maps as background map, makes the background non-transparent, makes the map movable by placing a 640x640 viewport over the map, forces the video to be 120000ms (2 minutes) long, makes the dot trail 10000ms (10 seconds) long, pre-draws the full track in grey (RGB color code #808080), hides the attribution overlay, and places the default information (lat/lng, speed, time) overlay at the bottom left. Output is stored in `movie.mp4`.

```bash
java -jar ./build/libs/gpx-animator-x.y.z-all.jar
	  --tms-url-template 'https://mt1.google.com/vt/lyrs=m&x={x}&y={y}&z={zoom}'
	  --background-map-visibility 1.0
	  --viewport-height 640 --viewport-width 640
	  --total-time 120000
	  --tail-duration 10000
	  --pre-draw-track --pre-draw-track-color '#808080'
	  --attribution-position hidden
	  --information-position 'bottom left'
	  --input input.gpx
	  --output movie.mp4
```
(where `x.y.z` refers to the version of the jar you built or downloaded)

## Contributors

Special thanks for all the people who had helped this project so far:

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://fihlon.swiss/"><img src="https://avatars.githubusercontent.com/u/1254039?v=4?s=100" width="100px;" alt="Marcus Fihlon"/><br /><sub><b>Marcus Fihlon</b></sub></a><br /><a href="#projectManagement-McPringle" title="Project Management">📆</a> <a href="#ideas-McPringle" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/gpx-animator/gpx-animator/commits?author=McPringle" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/zdila"><img src="https://avatars.githubusercontent.com/u/636095?v=4?s=100" width="100px;" alt="Martin Ždila"/><br /><sub><b>Martin Ždila</b></sub></a><br /><a href="#projectManagement-zdila" title="Project Management">📆</a> <a href="#ideas-zdila" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/gpx-animator/gpx-animator/commits?author=zdila" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://retiredtechie.fitchfamily.org/"><img src="https://avatars.githubusercontent.com/u/4681938?v=4?s=100" width="100px;" alt="n76"/><br /><sub><b>n76</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=n76" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/markus-schmidlin"><img src="https://avatars.githubusercontent.com/u/13030829?v=4?s=100" width="100px;" alt="Markus Schmidlin"/><br /><sub><b>Markus Schmidlin</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=markus-schmidlin" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/martinfrancois"><img src="https://avatars.githubusercontent.com/u/14319020?v=4?s=100" width="100px;" alt="François Martin"/><br /><sub><b>François Martin</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=martinfrancois" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maebli"><img src="https://avatars.githubusercontent.com/u/1138612?v=4?s=100" width="100px;" alt="Maebli"/><br /><sub><b>Maebli</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=maebli" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rindy22"><img src="https://avatars.githubusercontent.com/u/56276884?v=4?s=100" width="100px;" alt="rindy22"/><br /><sub><b>rindy22</b></sub></a><br /><a href="#ideas-rindy22" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/gpx-animator/gpx-animator/commits?author=rindy22" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/bat-bloke"><img src="https://avatars.githubusercontent.com/u/57795480?v=4?s=100" width="100px;" alt="Andy Oakey"/><br /><sub><b>Andy Oakey</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=bat-bloke" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/fgaignat"><img src="https://avatars.githubusercontent.com/u/23083528?v=4?s=100" width="100px;" alt="fgaignat"/><br /><sub><b>fgaignat</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=fgaignat" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/charlysog"><img src="https://avatars.githubusercontent.com/u/63605339?v=4?s=100" width="100px;" alt="charlysog"/><br /><sub><b>charlysog</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Acharlysog" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/waschulte"><img src="https://avatars.githubusercontent.com/u/59023045?v=4?s=100" width="100px;" alt="waschulte"/><br /><sub><b>waschulte</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Awaschulte" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/SirCremefresh"><img src="https://avatars.githubusercontent.com/u/20863779?v=4?s=100" width="100px;" alt="Donato Wolfisberg"/><br /><sub><b>Donato Wolfisberg</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=SirCremefresh" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/galz10"><img src="https://avatars.githubusercontent.com/u/38544478?v=4?s=100" width="100px;" alt="Gal Zahavi"/><br /><sub><b>Gal Zahavi</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=galz10" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/poorlymac"><img src="https://avatars.githubusercontent.com/u/16620846?v=4?s=100" width="100px;" alt="poorlymac"/><br /><sub><b>poorlymac</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=poorlymac" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/antonio-barber-67273bba/"><img src="https://avatars.githubusercontent.com/u/21110513?v=4?s=100" width="100px;" alt="Antonio D Barber"/><br /><sub><b>Antonio D Barber</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=abarber7" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/herrwusel"><img src="https://avatars.githubusercontent.com/u/8242787?v=4?s=100" width="100px;" alt="herrwusel"/><br /><sub><b>herrwusel</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Aherrwusel" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rammmiro"><img src="https://avatars.githubusercontent.com/u/32325306?v=4?s=100" width="100px;" alt="Ramiro Martínez Pinilla"/><br /><sub><b>Ramiro Martínez Pinilla</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Arammmiro" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://www.futurewater.nl/"><img src="https://avatars.githubusercontent.com/u/12559676?v=4?s=100" width="100px;" alt="Peter Droogers"/><br /><sub><b>Peter Droogers</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Apdroogers" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/fwieringen"><img src="https://avatars.githubusercontent.com/u/4232879?v=4?s=100" width="100px;" alt="Friso van Wieringen"/><br /><sub><b>Friso van Wieringen</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Afwieringen" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://thomer.com/"><img src="https://avatars.githubusercontent.com/u/1020105?v=4?s=100" width="100px;" alt="Thomer Gil"/><br /><sub><b>Thomer Gil</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Athomergil" title="Bug reports">🐛</a> <a href="https://github.com/gpx-animator/gpx-animator/commits?author=thomergil" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mundry"><img src="https://avatars.githubusercontent.com/u/1453314?v=4?s=100" width="100px;" alt="mundry"/><br /><sub><b>mundry</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=mundry" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="http://blog.mrtrustor.net/"><img src="https://avatars.githubusercontent.com/u/2864678?v=4?s=100" width="100px;" alt="Théo Chamley"/><br /><sub><b>Théo Chamley</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=MrTrustor" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/triskaidekafeliks"><img src="https://avatars.githubusercontent.com/u/19534176?v=4?s=100" width="100px;" alt="triskaidekafeliks"/><br /><sub><b>triskaidekafeliks</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/commits?author=triskaidekafeliks" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/krugerk"><img src="https://avatars.githubusercontent.com/u/4656811?v=4?s=100" width="100px;" alt="krugerk"/><br /><sub><b>krugerk</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Akrugerk" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/piiskop"><img src="https://avatars.githubusercontent.com/u/14224528?v=4?s=100" width="100px;" alt="peacecop kalmer:"/><br /><sub><b>peacecop kalmer:</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Apiiskop" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rneppi"><img src="https://avatars.githubusercontent.com/u/28830856?v=4?s=100" width="100px;" alt="rneppi"/><br /><sub><b>rneppi</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Arneppi" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/szolnokit"><img src="https://avatars.githubusercontent.com/u/49479918?v=4?s=100" width="100px;" alt="szolnokit"/><br /><sub><b>szolnokit</b></sub></a><br /><a href="https://github.com/gpx-animator/gpx-animator/issues?q=author%3Aszolnokit" title="Bug reports">🐛</a></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td align="center" size="13px" colspan="7">
        <img src="https://raw.githubusercontent.com/all-contributors/all-contributors-cli/1b8533af435da9854653492b1327a23a4dbd0a10/assets/logo-small.svg">
          <a href="https://all-contributors.js.org/docs/en/bot/usage">Add your contributions</a>
        </img>
      </td>
    </tr>
  </tfoot>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

## Contributing

### Good First Issues

For your first contribution to this repository, you can take a look at the issues listed here: [Good first issue](https://github.com/gpx-animator/gpx-animator/contribute).

### Gitpod Online IDE

You can open this project in a preconfigured Gitpod online IDE based on Theia (Visual Studio Code) and edit, run, test, debug and commit directly from your browser.

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/gpx-animator/gpx-animator)

### Slack Channel

There is a public Slack channel for GPX Animator available, which is hosted by the [Java User Group Switzerland](https://www.jug.ch/). If you are not already a member of this workspace, you can request a free invitation link with your email address (and nothing more) here: [Join Slack Workspace.](http://slack.jug.ch/)

After you have entered the Slack Workspace, join the #gpx-animator channel.

## Build

GPX Animator uses the [Gradle](https://gradle.org/) build system to build a JAR file. You do not need Gradle installed on your system. This project uses the Gradle Wrapper.

```
./gradlew assemble
# successful build puts .jar file in build/libs/
```

After a successful build, the JAR file can be found in the `build/libs/` directory.

Tests can be temporarily skipped by running

```
./gradlew assemble -x test
```

## Run

To run GPX Animator from source:

```
./gradlew run
```

To run GPX Animator from source with command line parameters:

```
./gradlew run --args="--input ./src/test/resources/gpx/bikeride.gpx --output test.mp4"
```

If necessary, the project will be (re)compiled.

## Test

To run tests in `src/test/`:

```
./gradlew test
```

## Related projects

- [gopro-map-sync](https://github.com/thomergil/gopro-map-sync): uses GPX Animator to synchronize a moving map video with GoPro footage.

## Credits

Icons included in application and their source:

* Airplane icon made by [Freepik](https://www.flaticon.com/authors/freepik) from [flaticon](https://www.flaticon.com/).
* Bicycle icon made by [Freepik](https://www.flaticon.com/authors/freepik) from [flaticon](https://www.flaticon.com/).
* Bus icon made by [monkik](https://www.flaticon.com/authors/monkik) from [flaticon](https://www.flaticon.com/).
* Car icon made by [Smashicons](https://www.flaticon.com/authors/smashicons) from [flaticon](https://www.flaticon.com/).
* Jogging icon made by [Freepik](https://www.flaticon.com/authors/freepik) from [flaticon](https://www.flaticon.com/).
* Riding icon made by [mynamepong](https://www.flaticon.com/authors/mynamepong) from [flaticon](https://www.flaticon.com/).
* Sailing icon made by [Freepik](https://www.flaticon.com/authors/freepik) from [flaticon](https://www.flaticon.com/).
* Ship icon made by [Freepik](https://www.flaticon.com/authors/freepik) from [flaticon](https://www.flaticon.com/).
* Tramway icon made by [Freepik](https://www.flaticon.com/authors/freepik) from [flaticon](https://www.flaticon.com/).
* Train icon made by [Smashicons](https://www.flaticon.com/authors/smashicons) from [flaticon](https://www.flaticon.com/).
* Trekking icon made by [monkik](https://www.flaticon.com/authors/monkik) from [flaticon](https://www.flaticon.com/).
* Motorcycle icon made by [poorlymac](https://github.com/poorlymac) using images from [ducati](https://www.ducati.com/us/en/bikes/multistrada)

Sounds included in application and their source:

* Success sound made by [nckn](https://freesound.org/people/nckn/sounds/256113/) from [freesound](https://freesound.org/)
* Error sound made by [lluiset7](https://freesound.org/people/lluiset7/sounds/141334/) from [freesound](https://freesound.org/)

To create the installers, we use a free license of [Install4J](https://www.ej-technologies.com/products/install4j/overview.html) for open-source projects.

[![Install4J multi-platform installer builder](https://www.ej-technologies.com/images/product_banners/install4j_large.png)](https://www.ej-technologies.com/products/install4j/overview.html)
