# Smart Campus Navigation System (MRIIRS)

```
campus/
├── CMakeLists.txt
├── main.cpp                 C++ REST API + Dijkstra (Crow)
└── frontend/
    ├── index.html
    ├── css/style.css
    └── js/
        ├── campus-config.js  <- edit locations / coordinates here
        └── app.js
```

## Run
```
cd campus
cmake -S . -B build
cmake --build build
./build/campus_server        # Windows: build\Release\campus_server.exe (or build\campus_server.exe)
```
Open http://localhost:18080 . Internet is needed for the map tiles and the Leaflet library.
Without the server, the page still works (browser Dijkstra fallback) if opened via any static server.
