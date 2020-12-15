# Optimize

Download imagemagick

```bash
# Create thumbprint
 magick convert .\michael-jin-mCj7atG0nEc-unsplash.jpg -quality 65 -strip -resize "1920x780" michael-jin-mCj7atG0nEc-unsplash_thumb.jpg

# Optimize image
magick convert .\michael-jin-mCj7atG0nEc-unsplash.jpg -quality 100 -strip -resize "1920x780" michael-jin-mCj7atG0nEc-unsplash.jpg
```