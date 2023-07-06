# [Properties](https://learn.microsoft.com/en-us/dotnet/csharp/properties)
Implements field with **getter** and **setter** accessors.

```c#
public class Person
{
    public string? FirstName { get; private set; }
}
```

You can also define the accessors

```c#
public class Person
{
    public string? FirstName
    {
        get { return _firstName; }
        set { _firstName = value; }
    }
    private string? _firstName;
}
```
