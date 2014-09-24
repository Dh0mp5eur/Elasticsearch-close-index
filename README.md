Elasticsearch-close-index
=========================

A script to close Elasticsearch indices
========================

$ ./elasticsearch-close-index --help

Usage: elasticsearch-close-index [ OPTIONS ]

Options:

-H, --host <host:port>
    The host and port name of the elasticsearch instance.
    Default: 127.0.0.1:9200
-p, --proto <http|https>
    Use http or https to connect to elasticsearch.
    Default: http
-a, --auth <username:password>
    Pass a string to auth via auth basic.
-i, --index <index> Base name of index index-YY.MM.DD
    Default: logstash-YY.MM.DD.
-c, --close <days>
    Close all indexes that are older than --close days.
-r, --run
    This parameter must be set to really close indices.
    If the parameter is not set then the indices are printed to
    stdout that would be closed if the parameter --run were set.
-h, --help
    Print the help.
