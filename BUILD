cc_library(
    name = "laslib",
    srcs = glob([
        "LASlib/src/*.cpp",
        "LASzip/src/*.cpp",
    ], exclude = [
        "LASlib/src/*dll*.cpp",
        "LASlib/src/*dll*.c",
        "LASzip/src/*dll*.cpp",
        "LASzip/src/*dll*.c",
    ]) + ["LASlib/inc/lasreader.hpp"],
    hdrs = glob([
        "LASlib/inc/*.hpp",
        "LASlib/inc/*.h",
        "LASlib/src/*.hpp",
        "LASlib/dll/*.h",
        "LASzip/src/*.hpp",
        "LASzip/src/*.h",
        "LASzip/include/laszip/*.h",
        "LASzip/dll/*.h",
    ]),
    includes = [
        "LASlib/inc",
        "LASlib/src",
        "LASlib/dll",
        "LASzip/src",
        "LASzip/include/laszip",
    ],
    linkopts = ["-ldl"],
    visibility = ["//visibility:public"],
)
