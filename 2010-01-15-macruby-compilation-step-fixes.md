Title: MacRuby compilation step fixes
Date: 2010-01-15 23:30:00
Slug: 2010/01/15/macruby-compilation-step-fixes
Tags: macruby, ruby, xcode, code, osx


Just a note, mostly to myself: The default XCode MacRuby `rb_main.rb` template
will contain these lines:


    Dir.entries(dir_path).each do |path|
      if path != File.basename(__FILE__) && path.match(/\.rb$/)
        require(path)
      end
    end


Works fine for uncompiled files, but when you want to compile your app,
there'll be no `*.rb` files — just `*.rbo` files. So `rb_main.rb` needs to be
adjusted.


    Dir.entries(dir_path).each do |path|
      if path != File.basename(__FILE__) && path.match(/\.rbo?$/)
        require(path)
      end
    end


I just spent 15 minutes wondering about these `Unknown class 'Controller',
using 'NSObject' instead. Encountered in Interface Builder file at path …` in
my system log, and I tend to forget this kind of detail so I wanted to jot it
down as a reminder to future Carlo.

So, listen up, future Carlo. This is _important_.
