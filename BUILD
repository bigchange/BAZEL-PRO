# example
# optimize bazel (分解项目)

java_binary(
    name = "my-runner",
    srcs = ["src/main/java/com/example/ProjectRunner.java"],
    main_class = "com.example.ProjectRunner",
    deps = [":greeter"],
)

java_library(
    name = "greeter",
    srcs = ["src/main/java/com/example/Greeting.java"],
    visibility = ["//visibility:public"], # BUILD目标可见选项设置
)
