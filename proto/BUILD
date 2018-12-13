load("@flow_protoc_gen//:defs.bzl", "flowtype_proto_library")
package(default_visibility = ["//visibility:public"])

filegroup(
  name = "proto_files",
  srcs = glob(["*.proto"]),
)

proto_library(
  name = "proto",
  srcs = [
    ":proto_files",
  ],
)

flowtype_proto_library(
  name = "generate",
  proto = ":proto",
)
