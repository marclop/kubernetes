load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "buffer.go",
        "certs.go",
        "channel.go",
        "cipher.go",
        "client.go",
        "client_auth.go",
        "common.go",
        "connection.go",
        "doc.go",
        "handshake.go",
        "kex.go",
        "keys.go",
        "mac.go",
        "messages.go",
        "mux.go",
        "server.go",
        "session.go",
        "streamlocal.go",
        "tcpip.go",
        "transport.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/golang.org/x/crypto/curve25519:go_default_library",
        "//vendor/golang.org/x/crypto/ed25519:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//vendor/golang.org/x/crypto/ssh/terminal:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
