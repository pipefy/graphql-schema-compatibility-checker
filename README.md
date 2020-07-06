[![CircleCI](https://circleci.com/gh/rodionovp/graphql-schema-compatibility-checker.svg?style=svg)](https://circleci.com/gh/rodionovp/graphql-schema-compatibility-checker)
# graphql-schema-compatibility-checker
A simple tool that checks if GraphQL schema is backward compatible.


# Installation
Install ammonite

    $ sudo curl -L -o /usr/local/bin/amm https://github.com/lihaoyi/Ammonite/releases/download/2.1.4/2.12-2.1.4 && sudo chmod +x /usr/local/bin/amm  

# Usage

## Check two schemas using retrospection query
    $ ./check-schema http://gdom.graphene-python.org/graphql http://gdom.graphene-python.org/graphql

## Check two local schemas in IDL format
    $ ./check-schema ./test/old-schema.graphql ./test/new-schema.graphql

Expected output:
```
 * Field `id` was removed from `Repository` type
```

          
