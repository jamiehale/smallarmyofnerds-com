[![CircleCI](https://circleci.com/gh/jamiehale/smallarmyofnerds-com.svg?style=svg)](https://circleci.com/gh/jamiehale/smallarmyofnerds-com)

# Small Army Of Nerds Site Code

This is the Jekyll code for the smallarmyofnerds.com site.

## Build

    $> bundle install
    $> bundle exec jekyll build

## Development

    $> bundle exec jekyll serve

## Test

    $> bundle exec htmlproofer ./_site --check-html --disable-external
