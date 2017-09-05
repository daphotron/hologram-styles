# hologram-styles
Hologram Default Style Files intended to be used with a vanilla instance of Middleman

# 1. CREATE MIDDLEMAN
```
middleman init [NAME_OF_PROJECT]
middleman build
middleman server
```

# 2. ADD HOLOGRAM GEM
…go into Gemfile, add `gem 'hologram'`
`bundle`

# 3. ADD TEST DOCUMENTATION
…open site.css.scss and add hologram documentation

# 4. CREATE STYLEGUIDE FOLDER
```
cd source
mkdir styleguide
```

# 5. INITIALIZE HOLOGRAM INSIDE STYLEGUIDE FOLDER
```
cd styleguide
hologram init
```

### 6A. OPTIONAL
replace styleguide folder with:
https://github.com/daphotron/hologram-styles

then skip to step # 7. RUN HOLOGRAM

# 6. CONFIGURE HOLOGRAM
…open hologram_config.yml
```
source: ../stylesheets
destination: ./
# - ./build
```

# 7. RUN HOLOGRAM
```
cd ../../
hologram source/styleguide/hologram_config.yml
```

# 8. VISIT YOUR STYLEGUIDE
/styleguide/index.html
