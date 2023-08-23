ADD_LIBRARY (absl_int128_clickhouse STATIC
    numeric/int128.cc
)

TARGET_INCLUDE_DIRECTORIES (absl_int128_clickhouse
    PUBLIC ${PROJECT_SOURCE_DIR}/contrib/absl
)

ADD_LIBRARY (absl::int128 ALIAS absl_int128_clickhouse)
