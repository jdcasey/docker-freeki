Docker wrapper for [Freeki](https://github.com/jdcasey/freeki) that runs in editable (default) mode. If you have an existing content repository, it can clone that before starting.

To run with a pre-existing content repository:

    docker run -e URL=https://github.com/myuser/mucontent.git -d -p 8080:8080 buildchimp/docker-freeki-readonly

To run with a new wiki (not pushable without extra manual steps!):

    docker run -d -p 8080:8080 buildchimp/docker-freeki-readonly
