A Github Pages template for academic websites. This was forked (then detached) by [Stuart Geiger](https://github.com/staeiou) from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License. See LICENSE.md.

I think I've got things running smoothly and fixed some major bugs, but feel free to file issues or make pull requests if you want to improve the generic template / theme.

### Note: if you are using this repo and now get a notification about a security vulnerability, delete the Gemfile.lock file. 

# Instructions

1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section
1. (Optional) Use the Jupyter notebooks or python scripts in the `markdown_generator` folder to generate markdown files for publications and talks from a TSV file.

See more info at https://academicpages.github.io/

## To run locally (not on GitHub Pages, to serve on your own computer)

1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll liveserve` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.

## Notes for myself

1. The homepage style and displayed items on the left (google scholoar, linkedin, twitter...) can be edited [here](https://github.com/Sheng-Cheng/Sheng-Cheng.github.io/blob/master/_config.yml)
1. The tabs on top can be managed [here](https://github.com/Sheng-Cheng/Sheng-Cheng.github.io/blob/master/_data/navigation.yml)
1. Current tabs can be edited in the .md files under /_pages: [homepage](https://github.com/Sheng-Cheng/Sheng-Cheng.github.io/blob/master/_pages/about.md), [Publications](https://github.com/Sheng-Cheng/Sheng-Cheng.github.io/blob/master/_pages/publications.md), [Teaching](https://github.com/Sheng-Cheng/Sheng-Cheng.github.io/blob/master/_pages/teaching.md), and Talks (still under construction and need to set up a .md file instead of .html.)
1. Research is a little special, where the html file [research.html](https://github.com/Sheng-Cheng/Sheng-Cheng.github.io/blob/master/_pages/research.html) defines how the [research page](https://sheng-cheng.github.io/research/) looks like. The entries to the research webpage are defined by the markdown files under [_research](https://github.com/Sheng-Cheng/Sheng-Cheng.github.io/tree/master/_research). You can use the [2023_difftune.md](https://github.com/Sheng-Cheng/Sheng-Cheng.github.io/blob/master/_research/2023_difftune.md) as an example (this one contains richest elements so far) to create new projects. Just remember to begin the file name with the year of completion so that the list can be arranged accordingly.


# Changelog -- bugfixes and enhancements

There is one logistical issue with a ready-to-fork template theme like academic pages that makes it a little tricky to get bug fixes and updates to the core theme. If you fork this repository, customize it, then pull again, you'll probably get merge conflicts. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch. 

To support this, all changes to the underlying code appear as a closed issue with the tag 'code change' -- get the list [here](https://github.com/academicpages/academicpages.github.io/issues?q=is%3Aclosed%20is%3Aissue%20label%3A%22code%20change%22%20). Each issue thread includes a comment linking to the single commit or a diff across multiple commits, so those with forked repositories can easily identify what they need to patch.
