# AlpineReflex

This app is a MVCE for issue [hopsoft/stimulus_reflex#329](https://github.com/hopsoft/stimulus_reflex/issues/329).


These are the commands to recreate this app:

```
rails new alpine_reflex --webpacker
cd alpine_reflex

bundle exec rails webpacker:install:stimulus
bundle exec rails g controller home index

bundle add stimulus_reflex
bundle exec rails stimulus_reflex:install
rails dev:cache

rails g stimulus_reflex example hello

yarn add alpinejs
```
