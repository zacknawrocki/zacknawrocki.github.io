# zacknawrocki.github.io
Personal website and virtual business card <br><br>


To create blogs or webpages, this website uses Gitfolio. Gitfolio can also tweak general settings.

### Setting Up Gitfolio

Install gitfolio

```sh
npm i gitfolio -g
```

Launch the UI

```sh
$ gitfolio ui
```

### Adding a Blog

Visit gitfolio server, assign configurations, and build.

```sh
http://localhost:3000
```

Select **New Blog** and fill out blog content. Gitfolio requires you to put in a background image. If you want the default background instead, put in a [random image](https://images.unsplash.com/photo-1547138666-12a241be3c2d?w) for now and proceed to the **Manual Tweaks, if Applicable** section, to remove the background image.

### Manual Tweaks, if Applicable

Within the resulting HTML blog file, you may want to make some custom tweaks. For example,

#### Use the Default Background Image on Your Blog Page

Remove

```
<div id="background_overlay"></div>
<div id="background" style="background: url(top_image.jpeg) center;"></div>
```

and replace with

```
<div id="background"></div>
```

#### Remove Gitfolio Footer

Remove

```
<div id="footer_blog">
  <a href="https://github.com/imfunniee" target="_blank">made on earth by a human</a>
</div>
```

#### Use a Favicon Different From Your GitHub Profile Picture

Remove

```
var icon = document.createElement("link");
icon.setAttribute("rel", "icon");
icon.setAttribute("href", user[0].userimg);
icon.setAttribute("type", "image/png");
document.getElementsByTagName("head")[0].appendChild(icon);
```

and add

```
<link rel="icon" href="../../media/img/icon.png" type="image/png"></head>

```
or a similar path to your Favicon image.







