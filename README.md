# oguzbilgic.com

my personal website

## Dependencies

### Ruby gems

Run the following to install the necessary gems:

    gem install jekyll rdiscount compass

### Pygments

Assuming you have python installed with `easy_install` available:

    sudo easy_install Pygments

## Rake deploy task

The following tasks are available (use `rake -T` to list them):

    rake build        # Build site with Jekyll
    rake check_links  # Check links for site already running on localhost:4000
    rake clean        # Clean up generated site
    rake deploy       # Build and deploy
    rake server       # Start server with --auto
