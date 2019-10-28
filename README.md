# bay

Bay is a simple theme for Jekyll. [[view live]](https://eliottvincent.github.io/bay)

Inspired by [dangrover.com](http://dangrover.com/). Current theme used at https://eliottvincent.com.

![](/screenshot.png)

### Installation

Create a new Jekyll website:
```
jekyll new mysite
```

Open `Gemfile` and replace the line:
```
gem "minima"
```
with:
```
gem "bay_jekyll_theme", "~> 1.0.8"
```

Open `_config.yml` and replace the line:
```
theme: minima
```
with:
```
theme: bay_jekyll_theme
```

Finally, install the dependencies:
```
bundle install
```

and build the website!
```
jekyll serve
```


The website will look somewhat empty at first. That's normal. Follow the next instructions to complete the header and footer components, and the home and blog pages.

### Header
Open the `_config.yml` file and add the following:
```yml
header:
  pages:
    - name: Home
      slug: /     # <-- index.md
    - name: Blog  # <-- blog.md
    - name: Whatever  # <-- whatever.md
```
Re-run `jekyll serve` to see the header updated.

### Footer
Open the `_config.yml` file and add the following:
```yml
footer:
  show_powered_by: true
  contact:
    - name: Email
      value: yourmail@domain.com
      link: mailto:yourmail@domain.com
    - name: WeChat
      value: YourWeChatUsername
      link: "#"
  follow:
    - name: Twitter
      link: http://twitter.com/YourTwitterUsername
      username: "@YourTwitterUsername"
    - name: Facebook
      link: http://facebook.com/YourFacebookUsername
    - name: LinkedIn
      link: http://linkedin.com/in/YourLinkedInUsername
    - name: GitHub
      link: http://github.com/YourGitHubUsername
    - name: Weibo
      link: http://weibo.com/u/YourWeiboUsername
```
Re-run `jekyll serve` to see the footer updated.

### Home page
Create (or edit) the `index.markdown` file and add the following:
```yml
---
layout: home
profile_picture:
  src: /assets/img/profile-pic.jpg
  alt: website picture
---

<p>
  Welcome to mysite!
</p>
```

### Blog page
Create `blog.markdown` file and add the following:
```yml
---
layout: blog
title: Blog
slug: /blog
---

This is an example of a "Blog" page, displaying a list of posts.
<br />
```


Your website is ready!