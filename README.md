# ruthieellis.github.io
This is the GitHub repoistory for the [Makey Cakey blog](https://ruth.ellis.scot/). The site is hosted on [GitHub Pages](https://pages.github.com/) using the [Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/). The blog was imoported from [http://makey-cakey.blogspot.com/](http://makey-cakey.blogspot.com/). 

# Create a new post
* Go to [https://github.com/ruthieellis/ruthieellis.github.io/tree/master/_posts](https://github.com/ruthieellis/ruthieellis.github.io/tree/master/_posts) 
* Click "Create new file"
* Name the file in the yyyy-mm-dd-post-title.md format 
* Add the following header:
```
---
title: Post title
tags:
- dairy free
- picnic
- dried fruit
header:
  teaser: "/assets/yyyy-mm-dd-image-0000.jpg"
---
Start your blog post here

```
* Posts are written in Markdown - [read more here](https://mmistakes.github.io/minimal-mistakes/markup/markup-html-tags-and-formatting/)

# Edit an old posts
Old posts are HTML format and may have broken links or missing external images. To edit, edit the file from the [posts](https://github.com/ruthieellis/ruthieellis.github.io/tree/master/_posts) folder.

# Upload an image
* Go to [https://github.com/ruthieellis/ruthieellis.github.io/tree/master/assets](https://github.com/ruthieellis/ruthieellis.github.io/tree/master/assets)
* Upload files, ideally in this format (but it's not essential) or you can add to a folder by year or year and month: 
```
/assets/yyyy-mm-dd-image-0000.jpg
```

You can also add an [image gallery](https://mmistakes.github.io/minimal-mistakes/docs/helpers/) - add the image links to the header and then embed the gallery in the post:

Header:
```
gallery:
  - url: /assets/2009-01-12-image-0002.JPG
    image_path: /assets/2009-01-12-image-0002.JPG
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: /assets/2009-01-12-image-0001.jpg
    image_path: /assets/2009-01-12-image-0001.jpg
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: /assets/2009-01-12-image-0000.jpg
    image_path: /assets/2009-01-12-image-0000.jpg
    alt: "placeholder image 3"
    title: "Image 3 title caption"
```


Body:
```
{% include gallery caption="This is a sample gallery with **Markdown support**." %}
```

# Add video
For YouTube:
```
{% include video id="XsxDH4HcOWA" provider="youtube" %}
```

For Vimeo:
```
{% include video id="212731897" provider="vimeo" %}
```

For Google Drive:
```
{% include video id="1u41lIbMLbV53PvMbyYc9HzvBug5lNWaO" provider="google-drive" %}
```

# Add an emoji
* The blog uses [https://github.com/jekyll/jemoji](https://github.com/jekyll/jemoji)
* Search for an emoji on [https://emojipedia.org/](https://emojipedia.org/)
* Copy the shortcode
* Add ```:+1:``` to your post to add a +1 emoji

# Redirects setup
The site has redirects from the old Blogger site to GitHub Pages. 
Notes:
* The original script (saved as scripts/script.rb) was from: [https://www.ybrikman.com/writing/2015/04/20/migrating-from-blogger-to-github-pages/](https://www.ybrikman.com/writing/2015/04/20/migrating-from-blogger-to-github-pages/)
* This script is saved as scripts/out-working.xml (and the original is scripts/out-original-incorrect.xml)
* To upload the redirects, go to Blogger and edit theme > Html here: [https://www.blogger.com/blogger.g?blogID=1766292537874588855#template](https://www.blogger.com/blogger.g?blogID=1766292537874588855#template)
* The regex used to replace URLs was ```ruth.ellis.scot(\/)(\/)\d{4}(\/)(((0)[0-9])|((1)[0-2]))(\/)([0-2][0-9]|(3)[0-1])(\/)```
* A backup of the original theme is saved as scripts/theme-backup.html
* The photo-a-day blog was imported from scripts/jekyll-photo-a-day.rb and scripts/blog-03-20-2019.xml
* The makey-cakey blog was imported from scripts/jekyll-makey-cakey.rb and scripts/blog-01-27-2019.xml
* The scripts used to import images are stored as scripts/import_blogger_images* - version href3 was used to create a branch of the site which has the largest size of each Blogger image saved (see next point)

# Old Blogger images
* The blog has all of the images imported but some images need to be clicked in order to get to the larger version of the image. These larger versions are still on Blogger. There is a branch in GitHub which has imported these images. The images are stored here: ```https://github.com/ruthieellis/ruthieellis.github.io/tree/large-blogger-images/assets/large``` and the edited posts are stored here: ```https://github.com/ruthieellis/ruthieellis.github.io/tree/large-blogger-images/_posts```. These were not overwritten as it also affected non-Blogger images but the images are here should they be needed. 


# Future changes
* Set up a [Forestry CMS](https://forestry.io/)
