## The EmacsBoston Website

This is a standard Jekyll site hosted on GitHub. If you'd like to suggest any
changes to the site, feel free to file an issue or submit a pull request.

### Building the site

All the standard [Jekyll documentation][] applies.

First, make sure you've got Ruby installed. Once you do, you'll need `bundler`,
the Ruby package manager:

    $ gem install bundler

Next, `cd` into this site's directory and install its dependencies:

    $ bundle

You should now be ready to build the site. To run the site locally for testing:

    $ bundle exec jekyll serve -w

The Jekyll server should now be running at `localhost:4000`. The `-w` option
makes Jekyll watch for changes and rebuild automatically.

Once you're satisfied with your changes, just commit them to `master` and push.
GitHub will handle the building and deployment.

### Scheduling a new meetup or adding a new video

To add a new post, create a new file in the `_posts` directory with the
appropriate timestamped prefix. Just mimic an existing one and you should be
fine.

Make sure the `layout` header is correctly set to either `announcement` (for a
newly scheduled meetup) or `video`. For announcements, be sure to set the
`scheduled` header, too.

Location partials are listed in the `_includes` directory. It's easy to add
more.

The new post will be included in the RSS feed automatically when the site is
deployed.

If you're unsure about anything you're doing, feel free to open a PR and tag
`@hrs`, who'd be happy to take a look.

### Licensing

Feel free to fork this repo and use it to help bootstrap your own meetup! It's
licensed as [CC BY-SA 4.0][], so you can build on it and tweak it to your
heart's content so long as you release your changes, too.

[Jekyll documentation]: https://jekyllrb.com/docs/home/
[CC BY-SA 4.0]: http://creativecommons.org/licenses/by-sa/4.0/
