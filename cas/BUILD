load("@rules_rust//rust:defs.bzl", "rust_binary")

rust_binary(
    name = "cas",
    srcs = ["cas_main.rs"],
    deps = [
        "//cas/grpc_service:ac_server",
        "//cas/grpc_service:bytestream_server",
        "//cas/grpc_service:capabilities_server",
        "//cas/grpc_service:cas_server",
        "//cas/grpc_service:execution_server",
        "//cas/grpc_service:worker_api_server",
        "//cas/scheduler:default_scheduler_factory",
        "//cas/store",
        "//cas/store:default_store_factory",
        "//cas/worker:local_worker",
        "//config",
        "//util:common",
        "//util:error",
        "//util:metrics_utils",
        "@crate_index//:async-lock",
        "@crate_index//:clap",
        "@crate_index//:scopeguard",
        "@crate_index//:env_logger",
        "@crate_index//:futures",
        "@crate_index//:hyper",
        "@crate_index//:json5",
        "@crate_index//:parking_lot",
        "@crate_index//:prometheus-client",
        "@crate_index//:axum",
        "@crate_index//:tls-listener",
        "@crate_index//:tower",
        "@crate_index//:tokio",
        "@crate_index//:tonic",
        "@crate_index//:tokio-rustls",
        "@crate_index//:rcgen",
        "@crate_index//:rustls-pemfile",
    ],
)
