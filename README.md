
## Contributing to this project

The training labs are displayed using mkdocs so they can be easily published to GitHub pages.

Environment setup to deploy locally:

~~~bin/bash
  pip3 install -r requirements
~~~

Development:

After cloning this repo and during development check the changes. It will start the live-reloading docs server.

~~~bash
mkdocs serve
~~~

Publish:

~~~bin
mkdocs gh-deploy --force
~~~


Issues running the project?

1. On OSX, if you see the error below when running `mkdocs serve`
```
OSError: cannot load library 'gobject-2.0-0': dlopen(gobject-2.0-0, 0x0002): tried: 'gobject-2.0-0' (no such file), '/System/Volumes/Preboot/Cryptexes/OSgobject-2.0-0' (no such file), '/usr/lib/gobject-2.0-0' (no such file, not in dyld cache), 'gobject-2.0-0' (no such file), '/usr/lib/gobject-2.0-0' (no such file, not in dyld cache).  Additionally, ctypes.util.find_library() did not manage to locate a library called 'gobject-2.0-0'
```

run:
```
brew install pango libffi
export DYLD_FALLBACK_LIBRARY_PATH=/opt/homebrew/lib:$DYLD_FALLBACK_LIBRARY_PATH
```