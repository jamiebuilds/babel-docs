# C#/.NET

### Installation

Support for Babel in .NET is provided by the [ReactJS.NET](http://reactjs.net/)
project. The core library can be installed via NuGet:

```
Install-Package React.Core
```

### Usage

```csharp
var babel = ReactEnvironment.Current.Babel;
// Transpiles a file
// You can instead use `TransformFileWithSourceMap` if you want a source map too.
var result = babel.TransformFile("foo.js");
// Transpiles a piece of code
var result = babel.Transform("class Foo { }");
```

> For more information see http://reactjs.net.
