# Repository for EE538 Assignements and Projects

## Bazel basics
1. ### Build File

    A build file is needed for all libraries and main code

    Load the bazel definitions using 
    
    `load("@rules_cc//cc:defs.bzl", "cc_binary", "cc_library")`

    `cc_binary` is used for main files. Can have dependencies.

    `cc_library` is used for libraries to link with
    ### **Note:** Libraries can have user defined visibility using the `visibility` command
    Build using `bazel build /path/to/buildfile:name_of_library`


2.  ### Run
    Run using `bazel run /path/to/buildfile:name_of_binary`



