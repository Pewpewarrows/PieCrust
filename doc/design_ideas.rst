Usage:
    Add a Resource (inherit from default, child, or custom)
    Wire the resource to a data source
    Define any relationships to other Resources, and how to embed them
    Add an Accessor (likely just an http endpoint)
    Wire the accessor to your project (Django route, Flask route, etc)

Resources:
    Resource
    DjangoModelResource
    SQLAlchemyResource
    MongoKitResource

Validators

Authorization

Authentication

Commands (RPC):
    Command
    Object (group of commands with state)

Clients:
    (aware of RFC and Schema structure to auto-build client models)

Output based on Accepts:
    html (should be usable as full documentation)
    xml
    json
    yaml
    bplist
    plaintext
    protobuf
    thrift
    messagepack

Routers/Accessors?:
    http
    zeromq
    sockets
    file
    process
    thread

Prefer HTTP Headers, but allow some configuration via GET vars for convenience.
