# hologram-styles
Hologram Default Style Files intended to be used with a vanilla instance of Middleman

- [Hologram Example Site](https://trulia.github.io/hologram/)
- [Example Repository] (https://github.com/trulia/hologram-example)

# 1. Create Middleman Instance
```
middleman init [NAME_OF_PROJECT]
middleman build
middleman server
```

# 2. Add Hologram Gem
…go into Gemfile, add `gem 'hologram'`
```
bundle
```

# 3. Add test documentation
…open site.css.scss and add hologram documentation
```
category: basics
```

# 4. Create Styleguide Folder
```
cd source
mkdir styleguide
```

# 5. Initialize Hologram
```
cd styleguide
hologram init
```

# 6A. Optional: Replace Hologram files with this repository
replace styleguide folder with:
https://github.com/daphotron/hologram-styles

then skip to step # 7. RUN HOLOGRAM

# 6. Configure Hologram
…open hologram_config.yml
```
source: ../stylesheets
destination: ./
# - ./build
```

# 7. Run Hologram
```
cd ../../
hologram source/styleguide/hologram_config.yml
```

# 8. Visit your styleguide
/styleguide/index.html
