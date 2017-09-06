# hologram-styles
Hologram Default Style Files intended to be used with a vanilla instance of Middleman

- [Hologram Example Site](https://trulia.github.io/hologram/)
- [Example Repository](https://github.com/trulia/hologram-example)

## 0. Prep Tools
```
gem install middleman
gem install hologram
```

## 1. Create Middleman Instance
```
middleman init [NAME_OF_PROJECT]
cd [NAME_OF_PROJECT] // go into the project
middleman build
middleman server
```

## 2. Add Hologram Gem
- Open the file `[NAME_OF_PROJECT]/source/Gemfile`
- At the bottom of the file add:
```
gem 'hologram'
```
- Keep middleman server running
- Open a different terminal and run:
```
bundle
```

## 3. Add test documentation
- Visit the [hologram example site](https://trulia.github.io/hologram/) and copy and paste hologram documentation code or...
- Open the file `[NAME_OF_PROJECT]/source/site.css.scss` and add hologram documentation:
```
/*doc
---
title: Buttons
name: button
category: basics
---

Button styles:

`` ``` ``html_example
<button class="btn btn-default">Button</button>
`` ``` ``

*/
```

## 4. Create Styleguide Folder
This will be where hologram's source files will be generated
```
cd source
mkdir styleguide
```

## 5. Initialize Hologram Source Files
```
cd styleguide
hologram init
```

## 6A. Optional: Replace Hologram files with this repository
Replace the whole styleguide folder with:
https://github.com/daphotron/hologram-styles/tree/master/styleguide

then skip to step ## 7. RUN HOLOGRAM

## 6. Configure Hologram
…open hologram_config.yml
```
source: ../stylesheets // Where your Hologram documentation code lives
destination: ./ // Where Hologram Build files will go
## - ./build
```

## 7. Run Hologram
```
// If you are inside your styleguide source folder `[NAME_OF_PROJECT]/source/styleguide` run:
hologram hologram_config.yml

// If you are inside this path `[NAME_OF_PROJECT]/source/` run:
hologram source/styleguide/hologram_config.yml
```

## 8. Visit your styleguide
/styleguide/index.html

## 8A. Optional: Update Stylesheets with some pre-built code
Replace the whole stylesheets folder with:
https://github.com/daphotron/hologram-styles/tree/master/stylesheets

