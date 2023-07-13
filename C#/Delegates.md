# Delegates
Type of variable that contains a reference to one or multiple **methods**.

The methods stored in a delegate can then be invoked.

The methods must match the **parameter list** and **return type** of the defined delegate.

```c#
public delegate int PerformCalculation(int x, int y);
public PerformCalculation performCalc; // instansiate delegate

int MyFunc(int a, int b) {
    // see how the params and return type matches the delegate
}

performCalc += MyFunc; // add method to delegate
performCalc?.Invoke(); // invoke methods in delegate
```

<br>

## Events
---
Types of delegates where the subscribed functions cannot be overridden.
```c#
performCalc += MyFunc;
performCalc = OtherFunc; // throws an error
```
And can only be invoked by the class that instansiated the event.
```c#
public event EventHandler MyEvent; // EventHandler is a type of delegate

private void Update() {
    myEvent?.Invoke();
}
```
<br>

## Actions & Funcs
---
Allow the creation of delegates on a single line.

<br>

**Actions:** Delegates that have parameters but no return value
```c#
public event Action MyAction; // instance of Action
public event Action<int> MyIntAction; // instance that takes an int parameter
```
**Funcs:** Delegates that can have parameters and a return value
```c#
public event Func<int, float> MyIntFunc; // last parameter is the return value
```

<br>
