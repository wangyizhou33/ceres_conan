## Conan first

```bash
    # install conan (one-time)
    pip3 install conan

    conan install . --output-folder=build --build=missing
    # a lot of cmake files are generated in the build folder

    # before building 
    cd build
    source conanbuild.sh

    cmake .. -DCMAKE_TOOLCHAIN_FILE=conan_toolchain.cmake -DCMAKE_BUILD_TYPE=Release
    cmake --build . --config Release
```

