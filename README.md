# C++ Formatting/Style

- STL naming conventions.

```cpp
// not good
class FooBar
{
    void doSomething(); // also not good
};

// good
class foo_bar
{
    void do_something();
};
```

- No extra indentation for namespaces.

```cpp
namespace foo
{

class bar
{
    void baz() const;
};

}
```

- Use modifiers like `const`, `override`, `final`, etc. as much as possible to express intent. Prefer `constexpr` to `const`.

- Prefer `#if defined` to `#ifdef`, since the former is more flexible/readable.

- Only declare functions inline in header files if they are a simple get/set.
