# Calling a binay of a specific version of a gem

I never knew this exisited. It seems it is not documented anywhere and I have no idea how it works, but yes:

```cap _3.4.0_ stage deploy```

will actually load version ```3.4.0``` and not a newer or an older one. [`Reference`][reference]

[reference]: http://stackoverflow.com/questions/4061596/how-can-i-call-an-older-version-of-a-gem-from-the-commandline
