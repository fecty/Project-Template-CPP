# C++ Project Template

General C++ Project Template Directory. It is meant to be configured according to specific projects later on.

## Requirements

- [MinGW-W64-builds](https://www.mingw-w64.org/)
- C++17 or newer.
- VS Code(Optional) for pre-provided build/run tasks.

## File Structuure

- `src/` - Contains the main application source code.
  - `*.cpp` : General source code file.
- `include/` - Header files of static libraries/other source code files are placed here.
  - `*.hpp` : Any general .hpp file.
- `lib/` - Static archive libraries are placed here.
  - `*.a` : Any general .a file.
- `bin/` - Where compiled executables are generated.
  - `main.exe` : Executable file generated from main.cpp.
  - `*.exe` : Any general Executable.
- `tests\` - Contains source code files related to testing/other demos.
  - `*.cpp` : General test source code file.
- `assets/` - Media and other resources used by the application are stored here.
  - `*.jpg` - General .jpg file.
  - `*.ttf` - General .ttf file.
- `.vscode/` - VS Code Configuration files.
  - `tasks.json` : Defines build and run tasks for VS Code.
- `.gitignore` - Specifies to Git, which files/folders to not track.
- `README.md` - Contains Description of project.

## Build Process

### Building with VS Code

1. Open the project directory in VS Code.
2. Go to `Terminal` -> `Run Build Task`.
3. Output executable will be `bin/*.exe`.

### Building from Command Line

```shell
cd projectDirectory/
g++ -static -Iinclude -Llib src/main.cpp -o bin/main.exe
```
Make sure that `mingw-w64/bin` is included in the `PATH` so that `g++` is available in the cmd. Otherwise navigate manually.


### Running with VS Code

1. Open the project directory in VS Code.
2. After building, Go to `Terminal` -> `Run Task` -> `Run` to run the compiled program.
2. The `Build and Run` task combines building and running in sequence.

### Running from the Command Line

Navigate to the project root directory and run the executable from the `bin/` directory:

```sh
.\bin\main.exe
```

Or, for test executables:

```sh
.\bin\window_test.exe
```

## Static Libraries
```sh
lib/
```

## Test Programs and demonstrations
```sh
tests/
```
## Resources and Assets
```sh
assets/
```

## Notes
