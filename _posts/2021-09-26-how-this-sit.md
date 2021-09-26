---
layout: post
title: "How this site came up"
---

In last post I had said that I will "write a small article on how this site came together". Also it was supposed to be coming soon. It took more than 2 years to get to it. Lesson learned, I won't atleast say that anything is coming soon in this blog.

It had been so long since I got this site up and running that I forgot everything. Except that I had used Jekyll. So, in order to fulfill the promise I had to relearn everything again. Finally, I was able to recreate everything again and by reliving the experience I (almost) recalled how I had got it the last time.

Seems like last time I had verbatim followed <a href="http://jmcglone.com/guides/github-pages/" target="_blank">this</a> link. Also, probably, without understanding much as I was racing to get something out. This time I had slowed a bit and followed how everything was wired together using Jekyll.

Since Jekyll is dependent on Ruby we need to setup Ruby environment first. I did the following steps on a clean Ubuntu OS
```
1. sudo apt install ruby-full build-essential zlib1g-dev
  1.1. Above installs ruby and gems
2. Next setup gem related paths
  2.1. echo '# Install Ruby Gems to ~/gems' >> ~/.zshrc
  2.2. echo 'export GEM_HOME="$HOME/gems"' >> ~/.zshrc
  2.3. echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.zshrc
  2.4. source ~/.zshrc
3. gem install jekyll bundler
```

Above pre-requisites are also availble on the <a href="https://jekyllrb.com/docs/" target="_blank">Jekyll docs</a> page.

Next I completed the <a href="https://jekyllrb.com/docs/step-by-step/01-setup/" target="_blank">Jekyll step-by-step tutorial</a>. This was more than enough to get this up and running.

