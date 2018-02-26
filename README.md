# graphql-schema-compatibility-checker
A simple tool that checks if GraphQL schema is backward compatible.


# Installation
Install ammonite

    $ sudo curl -L -o /usr/local/bin/amm https://git.io/vAcDx && sudo chmod +x /usr/local/bin/amm  

# Usage

## Check two schemas using retrospection query
    $ ./check-schema.sc http://gdom.graphene-python.org/graphql http://gdom.graphene-python.org/graphql

## Check two local schemas in IDL format
    $ ./check-schema.sc ./test/old-schema.graphql ./test/new-schema.graphql

Expected output:
```
 * Field `id` was removed from `Repository` type
```

          
