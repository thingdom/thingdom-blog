# Thingdom Blog


## Development

    jekyll --auto --server


## Deployment

    mv .git .git-bak    # hide .git repository from dotcloud
    rm -rf _site/       # delete old site (optional)
    jekyll              # generate new site
    dotcloud push thingdom.blog _site/

    # wait until this command finishes (FIXME)

    mv .git-bak .git    # restore .git repository
