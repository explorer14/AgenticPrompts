This C# repository uses Ports and Adapters style architecture and the code lives in the `src` folder. The  `Domain` project contains all the domain/business logic and its infrastructure agnostic.

`adapters` folder contains all the technology specific adapters that the core application uses.

`tests` folder contains all the tests for the application. We use `xUnit` test framework with `FluentAssertions` Nuget packeg version 7.x only and `Moq` Nuget package for mocking dependencies. 

Domain projects are never allowed to reference adapters or web service porjects directly. All the new types defined in the domain projects MUST always be `internal` and `sealed` by default.

All new C# interfaces created should always have XML documentation created that explains the purpose of the method and MUST also include any exceptions that the implementations of that interface are expected to throw.