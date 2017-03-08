# Elegant Theme - Improved

Responsive theme for [JsonResume](https://jsonresume.org/) inspired by card layouts.

Original [Theme Preview](http://themes.jsonresume.org/elegant)

Original [Theme Repository](https://github.com/mudassir0909/jsonresume-theme-elegant)

### Improved Version

The version from this repository has some improvements of two types:
- Generic changes/improvements (backwards compatible with the official JSON Resume repos and the original theme)
- Specific (such as new supported JSON fields and formats and their template representations), but from which anyone can benefit by checking the related forks and repositories:
  - [resume-schema fork](https://github.com/lmserrano/resume-schema)

Also, one of the goals of this repository is that all the information is put into the same single file, so that it can be properly exported and used in a normal offline CV file, if desired

This offline export can be achieved using [resume-builder](https://github.com/lmserrano/resume-builder)

The list of added features is as follows:
- Added total working time
- Added tags to profile
- Added `certificates` section
- Added `projects` section
- Make `projects` section collapsible
- Add scrolling capabilities to floating nav bar
- Added `other_skills` section
- Fonts are now embedded as base 64 into the template exported/rendered html files

For additional information, please check the "release-notes.md" file

### Markdown Supported
Only in the following places of now `resume.basics.summary`, `work[0].summary`, `work[0].highlights`, `education[0].courses`, `volunteer[0].summary`, `volunteer[0].highlights`, `awards[0].summary`, `publications[0].summary`, `references[0].reference`. If you have any other usecase, please raise an issue

### Social Profiles
The profiles are shown in the order in which they are specified in the `basics.profiles` array. By default, only 5 profiles are shown & others are revealed on demand.

![Profile Section](https://raw.githubusercontent.com/mudassir0909/jsonresume-theme-elegant/master/screenshots/profile.png)

#### Supported Profiles
* angellist
* behance
* bitbucket
* blogger
* codepen
* dribbble
* dribble
* exercism
* facebook
* flickr
* foursquare
* github
* googleplus
* gratipay
* hackernews
* instagram
* lastfm
* linkedin
* medium
* meetup
* pinterest
* reddit
* skype
* soundcloud
* spotify
* stackexchange
* stackoverflow
* telegram
* tumblr
* twitter
* vimeo
* youtube

### Credits
* Thank you [contributors](https://github.com/mudassir0909/jsonresume-theme-elegant/graphs/contributors) for your pull requests
* Floating Menu: inspired by [Smart Fixed Navigation](http://codyhouse.co/demo/smart-fixed-navigation/index.html)

### Contributing
```
$ git clone https://github.com/mudassir0909/jsonresume-theme-elegant.git
$ cd jsonresume-theme-elegant
$ npm install
$ grunt watch // watches for less file changes
$ grunt exec:run_server // Do this in a new terminal tab to run node server
```

Visit [http://localhost:8888](http://localhost:8888) to see the theme in action.

[![Throughput Graph](https://graphs.waffle.io/mudassir0909/jsonresume-theme-elegant/throughput.svg)](https://waffle.io/mudassir0909/jsonresume-theme-elegant/metrics)

##### Testing JSON changes
You can test your changes by updating `resume.json` file inside `node_modules/resume-schema/` folder. You might want to rerun `grunt exec:run_server` whenever you make any changes to `resume.json`

##### Updating Styles
All the LESS files are organized under the folder `assets/less/`. Please go through the comments inside `theme.less` to find out which file to put your LESS changes. Grunt compiles `assets/less/theme.less` to `assets/css/theme.css` which is used eventually in the theme.

**_Please Do not make any changes inside `assets/css/theme.css`_**

##### Updating Javascript
All the javascript changes go into `index.js` which is responsible for rendering the theme.

##### Adding a new icon
Visit this [wiki page](https://github.com/mudassir0909/jsonresume-theme-elegant/wiki/Adding-a-new-icon)

### Roadmap

[https://github.com/mudassir0909/jsonresume-theme-elegant/labels/enhancement](https://github.com/mudassir0909/jsonresume-theme-elegant/labels/enhancement)
