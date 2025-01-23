# Services
**Services refer to a class that can read or write data**

These are registered within the Dependency Injector (DI) container, which then can be injected into components or other services

The DI Container has 3 different “lifetimes” that a service can be registered as

Singleton - 1 Whole Instance For The Whole App

Scoped (Only used in server apps) - One instance per server request

Transient - Instance for each time it is injected