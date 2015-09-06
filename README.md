# speak-to-the-natives

This project aims to provide simple examples of how to do things with Elm's Natives. Elm's natives are [undocumented on purpose](https://groups.google.com/forum/#!topic/elm-discuss/DPuUPv72abc) and subject to change. While Elm is currently a solid way of creating web projects, there is still limited functionality that is best aided by reaching out into JS and either interecting with the DOM or performing some strange JS function that currently has no wrapper in Elm.

[Ports](http://elm-lang.org/guide/interop#ports) are already a way of interecting with JS. However, it is limited compared the accesibility possible through using Natives. If something is defined as a function through natives, then it is simpler for the developer to understand - there's no need to introduce the ports keyword, nor have any level of JS if your API is well defined. Ports currently support a limited set of types to be sent through them - while you can send records and JSON values, sometimes it's nicer to just send Dicts when you need them.

```
The types of values that can flow through outbound ports include:
Ints, Floats, Bools, Strings, Maybes, Lists, Arrays, Tuples,
Json.Values, and concrete records.
```

Any examples here exist only as a discussion point - they aren't to be used in the real world. In the Maths module, I have put purposely badly-named functions such as adding/subtracting so they are clearly not part of Basics or anything other real module.
