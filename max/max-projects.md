# Max Projects

Max projects aggressively manage files.

For example:

```
- Foo
    - Foo.maxproj
    - Foo.png
```

Will be converted to:

```
- Foo
    - Foo.maxproj
    - Media
        - Foo.png
```

For this reason, non-project related files, such as `README.md`, should not go in the project root.

## Project Window

- Files local to a project are shown in regular, non-italic text. Dependencies of project files are shown in a darker color, and if those files are only found on the global Max search path, they are shown in italics. Dependencies cannot be removed from a project from the Project window.
