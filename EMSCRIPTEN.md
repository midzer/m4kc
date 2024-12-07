# Emscripten

## Build

```
./build.sh small
```

## Link

```
emcc -flto -O3 -fno-rtti -fno-exceptions *.o -o index.html -sUSE_SDL=2 -sASYNCIFY -sASYNCIFY_IGNORE_INDIRECT -sASYNCIFY_ONLY=@../../funcs.txt -sENVIRONMENT=web --closure 1 -sEXPORTED_RUNTIME_METHODS=['allocate']
```
