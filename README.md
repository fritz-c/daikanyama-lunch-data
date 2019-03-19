# Daikanyama Restaurant Info

### Optimizing images before sharing
```sh
# Resize new images to a width of 1000, if you want
# brew install imagemagick
# git ls-files --others --exclude-standard -x "(jpg|jpeg)$" -z | xargs -0 mogrify -resize 1000

# Get ImageOptim
open https://imageoptim.com/mac
# Install ImageOptim CLI adapter
brew install imageoptim-cli
# Optimize image compression, shrink size and remove metadata from new images
git ls-files --others --exclude-standard -x "(jpg|jpeg)$" -z | xargs -0 imageoptim
```
