## segvcatch

This is a very simple and straight-forward crossplatform C++ library designed to convert a hardware exceptions or OS signals, such as segmentation fault, or floating point errors, into a software language exceptions, which can be handled later with a try/catch construction.

### Disclaimer

This repository contains sample code intended to demonstrate how to catch hardware signals. It is not intended to be used as-is in applications as a library dependency, and will not be maintained as such. Bug fix contributions are welcome, but issues and feature requests will not be addressed.

### Specifications

How to use this crossplatform structured exception handling (SEH).

For example, this code is working fine:

```c++
try {
    *(int*) 0 = 0;
} catch (std::exception& e) {
    std::cerr << "Exception catched : " << e.what() << std::endl;
}
```

### Contributing
If you would like to contribute code, you can do so through GitHub by forking the repository and sending a pull request.
When submitting code, please make every effort to follow existing conventions and style in order to keep the code as readable as possible.

## Credits

* [segvcatch][1]

## License

The code supplied here is covered under the MIT Open Source License..

[1]: https://code.google.com/archive/p/segvcatch/