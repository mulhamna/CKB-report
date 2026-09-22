```
cargo install ckb-cli
    Updating crates.io index
  Downloaded ckb-cli v1.4.0
  Downloaded 1 crate (1.4MiB) in 7.31s
  Installing ckb-cli v1.4.0
    Updating crates.io index
error: failed to compile `ckb-cli v1.4.0`, intermediate artifacts can be found at `/var/folders/h2/sxpb3_ld465dp1rflzh2fzk40000gn/T/cargo-installvNQ0sm`.
To reuse those artifacts with a future compilation, set the environment variable `CARGO_BUILD_BUILD_DIR` to that path.

Caused by:
  failed to select a version for the requirement `ckb-build-info = "=0.105.1"`
    version 0.105.1 is yanked
  location searched: crates.io index
  required by package `ckb-cli v1.4.0`
```

---

```
cargo install --git https://github.com/nervosnetwork/ckb-cli.git ckb-cli
    Updating git repository `https://github.com/nervosnetwork/ckb-cli.git`
  Installing ckb-cli v2.0.0 (https://github.com/nervosnetwork/ckb-cli.git#ebfedb28)
    Updating crates.io index
    Updating git repository `https://github.com/rust-bitcoin/rust-bitcoin`
     Locking 494 packages to latest compatible versions
      Adding aes-ctr v0.6.0 (available: v0.99.99)
      Adding ansi_term v0.11.0 (available: v0.12.1)
      Adding ckb-vm v0.24.14 (available: v0.24.15)
      Adding ckb-vm-definitions v0.24.14 (available: v0.24.15)
      Adding clap v3.0.0-beta.1 (available: v3.2.25)
      Adding clap_generate v3.0.0-beta.1 (available: v3.0.3)
      Adding colored v1.9.4 (available: v3.1.1)
      Adding console v0.15.11 (available: v0.16.6)
      Adding dirs v1.0.5 (available: v7.0.0)
      Adding dtoa v0.4.8 (available: v1.0.11)
      Adding env_logger v0.6.2 (available: v0.11.11)
      Adding faster-hex v0.6.1 (available: v0.10.0)
      Adding generic-array v0.14.7 (available: v0.14.9)
      Adding goblin v0.4.0 (available: v0.4.3)
      Adding ipnetwork v0.14.0 (available: v0.21.1)
      Adding parity-multiaddr v0.4.1 (available: v0.11.2)
      Adding parking_lot v0.11.2 (available: v0.12.5)
      Adding rand v0.7.3 (available: v0.10.3)
      Adding rpassword v3.0.2 (available: v7.5.4)
      Adding rustyline v14.0.0 (available: v18.0.1)
      Adding rustyline-derive v0.10.0 (available: v0.12.0)
      Adding scrypt v0.2.0 (available: v0.12.0)
      Adding secp256k1 v0.30.0 (available: v0.33.1)
      Adding serde_yaml v0.8.26 (available: v0.9.34+deprecated)
      Adding shell-words v0.1.0 (available: v1.1.1)
      Adding termion v1.5.6 (available: v4.0.6)
      Adding thiserror v1.0.69 (available: v2.0.20)
      Adding tiny-keccak v1.5.0 (available: v2.0.2)
      Adding toml v0.5.11 (available: v1.1.6+spec-1.1.0)
      Adding tui v0.6.2 (available: v0.19.0)
      Adding url v1.7.2 (available: v2.5.8)
      Adding uuid v0.7.4 (available: v1.26.1)
  Downloaded async-iterator v2.3.0
  Downloaded rand_pcg v0.1.2
  Downloaded aes-ctr v0.6.0
  Downloaded digest v0.8.1
  Downloaded derive-getters v0.2.1
  Downloaded ckb-channel v1.2.1
  Downloaded instant v0.1.13
  Downloaded jsonrpc-core v18.0.0
  Downloaded sha-1 v0.8.2
  Downloaded endian-type v0.1.2
  Downloaded rand_core v0.3.2
  Downloaded proc-macro-crate v0.1.5
  Downloaded parity-multihash v0.1.3
  Downloaded subtle v1.0.0
  Downloaded ckb-build-info v1.1.1
  Downloaded fd-lock v4.0.4
  Downloaded crypto-mac v0.7.0
  Downloaded jsonrpc-server-utils v18.0.0
  Downloaded percent-encoding v1.0.1
  Downloaded ipnetwork v0.14.0
  Downloaded byte-tools v0.3.1
  Downloaded numtoa v0.1.0
  Downloaded shell-words v0.1.0
  Downloaded hmac v0.7.1
  Downloaded jsonrpc-core-client v18.0.0
  Downloaded jsonrpc-client-transports v18.0.0
  Downloaded cipher v0.2.5
  Downloaded enum-repr-derive v0.2.0
  Downloaded rustyline-derive v0.10.0
  Downloaded autocfg v0.1.8
  Downloaded fake-simd v0.1.2
  Downloaded pbkdf2 v0.3.0
  Downloaded dirs v1.0.5
  Downloaded bech32 v0.8.1
  Downloaded vec_map v0.8.2
  Downloaded opaque-debug v0.2.3
  Downloaded block-buffer v0.7.3
  Downloaded rand_chacha v0.1.1
  Downloaded rand_hc v0.1.0
  Downloaded os_str_bytes v2.4.0
  Downloaded safemem v0.3.3
  Downloaded tiny-keccak v1.5.0
  Downloaded scrypt v0.2.0
  Downloaded rand_xorshift v0.1.1
  Downloaded keccak v0.1.6
  Downloaded dtoa v0.4.8
  Downloaded rpassword v3.0.2
  Downloaded unsigned-varint v0.2.3
  Downloaded clap_generate v3.0.0-beta.1
  Downloaded block-padding v0.1.5
  Downloaded ckb-util v1.3.1
  Downloaded rand_jitter v0.1.4
  Downloaded humantime v1.3.0
  Downloaded nibble_vec v0.1.0
  Downloaded colored v1.9.4
  Downloaded sha2 v0.8.2
  Downloaded generic-array v0.12.4
  Downloaded jsonrpc-http-server v18.0.0
  Downloaded net2 v0.2.39
  Downloaded ctr v0.6.0
  Downloaded rand_os v0.1.3
  Downloaded textwrap v0.11.0
  Downloaded env_logger v0.6.2
  Downloaded jsonrpc-derive v18.0.0
  Downloaded parking_lot_core v0.8.6
  Downloaded clap_derive v3.2.25
  Downloaded rand_core v0.4.3
  Downloaded rand_isaac v0.1.1
  Downloaded parity-multiaddr v0.4.1
  Downloaded base64 v0.9.3
  Downloaded parking_lot v0.11.2
  Downloaded yaml-rust v0.4.5
  Downloaded ansi_term v0.11.0
  Downloaded hex-conservative v0.3.2
  Downloaded bs58 v0.2.5
  Downloaded jsonrpc-pubsub v18.0.0
  Downloaded serde_yaml v0.8.26
  Downloaded termion v1.5.6
  Downloaded blake2 v0.8.1
  Downloaded uuid v0.7.4
  Downloaded tokio-util v0.6.10
  Downloaded url v1.7.2
  Downloaded bech32 v0.11.1
  Downloaded aes-soft v0.6.4
  Downloaded rand v0.6.5
  Downloaded itertools v0.8.2
  Downloaded rustyline v14.0.0
  Downloaded tui v0.6.2
  Downloaded clap v3.0.0-beta.1
  Downloaded rand v0.5.6
  Downloaded radix_trie v0.2.1
  Downloaded idna v0.1.5
  Downloaded sha3 v0.8.2
  Downloaded sha3 v0.10.9
  Downloaded ckb-system-scripts v0.6.0
  Downloaded ckb-sdk v5.1.0
  Downloaded bitcoinconsensus v0.106.0+26.0
  Downloaded 97 crates (10.5MiB) in 18.89s (largest was `bitcoinconsensus` at 4.0MiB)
   Compiling proc-macro2 v1.0.107
   Compiling unicode-ident v1.0.26
   Compiling quote v1.0.47
   Compiling libc v0.2.189
   Compiling serde_core v1.0.229
   Compiling serde v1.0.229
   Compiling cfg-if v1.0.5
   Compiling zerocopy v0.8.57
   Compiling getrandom v0.1.16
   Compiling shlex v2.0.1
   Compiling memchr v2.8.3
   Compiling find-msvc-tools v0.1.13
   Compiling version_check v0.9.5
   Compiling cc v1.4.7
   Compiling zmij v1.0.23
   Compiling syn v1.0.109
   Compiling thiserror v1.0.69
   Compiling itoa v1.0.18
   Compiling blake2b-rs v0.2.0
   Compiling faster-hex v0.6.1
   Compiling typenum v1.20.1
   Compiling pin-project-lite v0.2.17
   Compiling ref-cast v1.0.27
   Compiling syn v3.0.6
   Compiling syn v2.0.119
   Compiling rand_core v0.5.1
   Compiling serde_json v1.0.151
   Compiling rand_pcg v0.2.1
   Compiling heapsize v0.4.2
   Compiling futures-core v0.3.34
   Compiling once_cell v1.21.4
   Compiling serde_derive_internals v0.30.0
   Compiling smallvec v1.16.1
   Compiling serde_derive v1.0.229
   Compiling thiserror-impl v1.0.69
   Compiling ref-cast-impl v1.0.27
   Compiling schemars_derive v1.2.2
   Compiling ppv-lite86 v0.2.21
   Compiling autocfg v1.5.1
   Compiling rand_chacha v0.2.2
   Compiling crc32fast v1.5.2
   Compiling rand v0.7.3
   Compiling futures-sink v0.3.34
   Compiling numext-constructor v0.1.6
   Compiling anyhow v1.0.104
   Compiling siphasher v0.3.11
   Compiling dyn-clone v1.0.20
   Compiling synstructure v0.14.0
   Compiling siphasher v1.0.3
   Compiling log v0.4.34
   Compiling unicode-xid v0.2.6
   Compiling derive_more-impl v1.0.0
   Compiling phf_shared v0.12.1
   Compiling futures-channel v0.3.34
   Compiling fastrand v2.5.0
   Compiling zerofrom-derive v0.1.8
   Compiling phf_generator v0.12.1
   Compiling phf_shared v0.8.0
   Compiling futures-macro v0.3.34
   Compiling futures-task v0.3.34
   Compiling futures v0.1.31
   Compiling heck v0.5.0
   Compiling slab v0.4.12
   Compiling futures-io v0.3.34
   Compiling strum_macros v0.27.2
   Compiling phf_macros v0.12.1
   Compiling yoke-derive v0.8.3
   Compiling bytes v1.12.1
   Compiling ckb-occupied-capacity-core v1.1.1
   Compiling zerofrom v0.1.8
   Compiling schemars v1.2.2
   Compiling ckb-occupied-capacity-macros v1.1.1
   Compiling futures-util v0.3.34
   Compiling tokio-macros v2.7.2
   Compiling socket2 v0.6.5
   Compiling mio v1.2.3
   Compiling generic-array v0.14.7
   Compiling adler2 v2.0.1
   Compiling simd-adler32 v0.3.10
   Compiling stable_deref_trait v1.2.1
   Compiling cty v0.2.2
   Compiling bitflags v2.13.2
   Compiling paste v1.0.15
   Compiling yoke v0.8.3
   Compiling miniz_oxide v0.9.1
   Compiling tokio v1.53.1
   Compiling numext-fixed-uint-core v0.1.6
   Compiling flate2 v1.1.10
   Compiling phf_generator v0.8.0
   Compiling zerovec-derive v0.11.6
   Compiling getrandom v0.2.17
   Compiling seq-macro v0.3.6
   Compiling same-file v1.0.6
   Compiling ckb-fixed-hash-core v1.1.2
   Compiling byteorder v1.5.0
   Compiling walkdir v2.5.0
   Compiling ckb-fixed-hash-macros v1.1.1
   Compiling phf_codegen v0.8.0
   Compiling displaydoc v0.2.7
   Compiling arrayvec v0.7.8
   Compiling includedir_codegen v0.6.0
   Compiling rand_core v0.4.3
   Compiling zerovec v0.11.8
   Compiling ckb-fixed-hash v1.1.1
   Compiling ckb-occupied-capacity v1.1.1
   Compiling derive_more v1.0.0
   Compiling cpufeatures v0.2.17
   Compiling rustix v1.1.5
   Compiling blake2b-ref v0.3.1
   Compiling ckb-hash v1.1.1
   Compiling phf v0.12.1
   Compiling molecule v0.9.2
   Compiling strum v0.27.2
   Compiling tinystr v0.8.4
   Compiling numext-fixed-uint-hack v0.1.6
   Compiling autocfg v0.1.8
   Compiling errno v0.3.14
   Compiling generic-array v0.12.4
   Compiling writeable v0.6.4
   Compiling numext-fixed-uint v0.1.6
   Compiling litemap v0.8.3
   Compiling potential_utf v0.1.6
   Compiling zerotrie v0.2.5
   Compiling futures-executor v0.3.34
   Compiling golomb-coded-set v0.2.1
   Compiling merkle-cbt v0.3.2
   Compiling ckb-merkle-mountain-range v0.5.2
   Compiling unicode-width v0.1.14
   Compiling utf8_iter v1.0.4
   Compiling icu_normalizer_data v2.3.0
   Compiling getrandom v0.4.3
   Compiling bit-vec v0.6.3
   Compiling icu_properties_data v2.3.0
   Compiling ckb-error v1.1.1
   Compiling ckb-constant v1.1.3
   Compiling icu_collections v2.3.0
   Compiling futures v0.3.34
   Compiling crypto-common v0.1.7
   Compiling block-buffer v0.10.4
   Compiling rand_core v0.3.2
   Compiling ckb-system-scripts v0.5.4
   Compiling core-foundation-sys v0.8.7
   Compiling scopeguard v1.2.0
   Compiling percent-encoding v2.3.2
   Compiling lock_api v0.4.14
   Compiling icu_locale_core v2.3.0
   Compiling digest v0.10.7
   Compiling ahash v0.7.8
   Compiling byte-tools v0.3.1
   Compiling ckb-rational v1.1.2
   Compiling ckb-gen-types v1.1.1
   Compiling bitcoin-io v0.1.101
   Compiling httparse v1.10.1
   Compiling icu_provider v2.3.1
   Compiling tempfile v3.27.0
   Compiling digest v0.8.1
   Compiling icu_properties v2.3.0
   Compiling rand_core v0.6.4
   Compiling http v1.5.0
   Compiling phf v0.8.0
   Compiling secp256k1-sys v0.10.1
   Compiling icu_normalizer v2.3.0
   Compiling proc-macro-error-attr v1.0.4
   Compiling try-lock v0.2.5
   Compiling bitcoin-internals v0.4.0 (https://github.com/rust-bitcoin/rust-bitcoin?rev=436de8ef12ab371aab6e9f6fbfb098238b42657d#436de8ef)
   Compiling tower-service v0.3.3
   Compiling idna_adapter v1.2.2
   Compiling http-body v1.1.0
   Compiling want v0.3.1
   Compiling includedir v0.6.0
   Compiling rand_chacha v0.3.1
   Compiling block-padding v0.1.5
   Compiling hex-conservative v0.2.3
   Compiling hex-conservative v0.3.2
   Compiling tracing-core v0.1.36
   Compiling proc-macro-error v1.0.4
   Compiling parking_lot_core v0.8.6
   Compiling lazy_static v1.5.0
   Compiling subtle v1.0.0
   Compiling opaque-debug v0.2.3
   Compiling crypto-mac v0.7.0
   Compiling tracing v0.1.44
   Compiling hashbrown v0.12.3
   Compiling bitcoin_hashes v0.14.101
   Compiling block-buffer v0.7.3
   Compiling rand v0.8.8
   Compiling idna v1.1.0
   Compiling form_urlencoded v1.2.2
   Compiling core-foundation v0.10.1
   Compiling security-framework-sys v2.17.0
   Compiling jsonrpc-core v18.0.0
   Compiling rand_chacha v0.1.1
   Compiling rand_pcg v0.1.2
   Compiling tokio-stream v0.1.19
   Compiling ckb-types v1.1.3
   Compiling scroll_derive v0.10.5
   Compiling miette-derive v5.10.0
   Compiling instant v0.1.13
   Compiling time-core v0.1.9
   Compiling num-conv v0.2.2
   Compiling native-tls v0.2.18
   Compiling parking_lot_core v0.9.12
   Compiling convert_case v0.4.0
   Compiling either v1.18.0
   Compiling derive_more v0.99.20
   Compiling miette v5.10.0
   Compiling scroll v0.10.2
   Compiling ckb-jsonrpc-types v1.2.0
   Compiling ckb-resource v1.2.0
   Compiling time-macros v0.2.32
   Compiling security-framework v3.7.0
   Compiling sha-1 v0.10.1
   Compiling secp256k1 v0.30.0
   Compiling sha2 v0.10.9
   Compiling rand v0.6.5
   Compiling keccak v0.1.6
   Compiling aho-corasick v1.1.5
   Compiling cookie v0.18.2
   Compiling hex v0.4.3
   Compiling plain v0.2.3
   Compiling fake-simd v0.1.2
   Compiling deranged v0.5.8
   Compiling powerfmt v0.2.0
   Compiling base64 v0.21.7
   Compiling regex-syntax v0.8.11
   Compiling xxhash-rust v0.8.18
   Compiling tinyvec v1.13.3
   Compiling atomic-waker v1.1.2
   Compiling time v0.3.55
   Compiling hyper v1.11.1
   Compiling ssri v9.2.0
   Compiling unicode-normalization v0.1.25
   Compiling regex-automata v0.4.18
   Compiling parking_lot v0.11.2
   Compiling ckb-traits v1.1.2
   Compiling url v2.5.8
   Compiling bitcoin_hashes v0.16.0 (https://github.com/rust-bitcoin/rust-bitcoin?rev=436de8ef12ab371aab6e9f6fbfb098238b42657d#436de8ef)
   Compiling sha1 v0.10.7
   Compiling rand_xorshift v0.1.1
   Compiling rand_isaac v0.1.1
   Compiling rand_hc v0.1.0
   Compiling rand_os v0.1.3
   Compiling rand_jitter v0.1.4
   Compiling indexmap v1.9.3
   Compiling sync_wrapper v1.0.2
   Compiling memmap2 v0.5.10
   Compiling ckb-vm v0.24.14
   Compiling reflink-copy v0.1.30
   Compiling ipnet v2.12.2
   Compiling ryu v1.0.23
   Compiling psl-types v2.0.11
   Compiling objc2 v0.6.4
   Compiling bitflags v1.3.2
   Compiling eaglesong v0.1.0
   Compiling litrs v1.0.0
   Compiling tower-layer v0.3.3
   Compiling base64 v0.22.1
   Compiling unicode-bidi v0.3.18
   Compiling matches v0.1.10
   Compiling document-features v0.2.12
   Compiling idna v0.1.5
   Compiling hyper-util v0.1.20
   Compiling tower v0.5.3
   Compiling ckb-pow v1.1.1
   Compiling publicsuffix v2.3.0
   Compiling cacache v13.1.0
   Compiling tokio-native-tls v0.3.1
   Compiling sha2 v0.8.2
   Compiling goblin v0.4.0
   Compiling goblin v0.2.3
   Compiling ckb-crypto v1.1.1
   Compiling ckb-dao-utils v1.1.1
   Compiling http-body-util v0.1.5
   Compiling cipher v0.2.5
   Compiling ckb-vm-definitions v0.24.14
   Compiling ckb-system-scripts v0.6.0
   Compiling toml v0.5.11
   Compiling ckb-logger v1.1.1
   Compiling num-traits v0.2.19
   Compiling crossbeam-utils v0.8.23
   Compiling ckb-script v1.2.0
   Compiling crunchy v0.2.4
   Compiling zeroize v1.9.0
   Compiling percent-encoding v1.0.1
   Compiling fnv v1.0.7
   Compiling cfg_aliases v0.1.1
   Compiling cfg_aliases v0.2.2
   Compiling objc2-encode v4.1.0
   Compiling nix v0.28.0
   Compiling http v0.2.12
   Compiling nix v0.31.3
   Compiling url v1.7.2
   Compiling ckb-chain-spec v1.1.2
   Compiling rustls-pki-types v1.15.1
   Compiling hyper-tls v0.6.0
   Compiling cookie_store v0.22.1
   Compiling tower-http v0.6.11
   Compiling serde_urlencoded v0.7.1
   Compiling bitcoin-units v0.2.0 (https://github.com/rust-bitcoin/rust-bitcoin?rev=436de8ef12ab371aab6e9f6fbfb098238b42657d#436de8ef)
   Compiling linked-hash-map v0.5.6
   Compiling iovec v0.1.4
   Compiling atty v0.2.14
   Compiling bstr v1.13.1
   Compiling hashbrown v0.14.5
   Compiling opaque-debug v0.3.1
   Compiling safemem v0.3.3
   Compiling termcolor v1.4.1
   Compiling heck v0.4.1
   Compiling base64 v0.9.3
   Compiling aes-soft v0.6.4
   Compiling clap_derive v3.2.25
   Compiling dashmap v5.5.3
   Compiling globset v0.4.20
   Compiling bitcoin-primitives v0.101.0 (https://github.com/rust-bitcoin/rust-bitcoin?rev=436de8ef12ab371aab6e9f6fbfb098238b42657d#436de8ef)
   Compiling bytes v0.4.12
   Compiling block2 v0.6.2
   Compiling http-body v0.4.6
   Compiling reqwest v0.12.28
   Compiling ctr v0.6.0
   Compiling base58ck v0.2.0 (https://github.com/rust-bitcoin/rust-bitcoin?rev=436de8ef12ab371aab6e9f6fbfb098238b42657d#436de8ef)
   Compiling bitcoin-io v0.2.0 (https://github.com/rust-bitcoin/rust-bitcoin?rev=436de8ef12ab371aab6e9f6fbfb098238b42657d#436de8ef)
   Compiling ckb-mock-tx-types v1.1.1
   Compiling jsonrpc-pubsub v18.0.0
   Compiling sha-1 v0.8.2
   Compiling sha3 v0.8.2
   Compiling sha3 v0.10.9
   Compiling enum-repr-derive v0.2.0
   Compiling lru v0.7.8
   Compiling blake2 v0.8.1
   Compiling hmac v0.7.1
   Compiling pbkdf2 v0.3.0
   Compiling iana-time-zone v0.1.65
   Compiling rand v0.5.6
   Compiling textwrap v0.11.0
   Compiling tokio-util v0.6.10
   Compiling tokio-util v0.7.19
   Compiling derive-getters v0.2.1
   Compiling async-trait v0.1.92
   Compiling nibble_vec v0.1.0
   Compiling socket2 v0.5.10
   Compiling ckb-build-info v1.1.1
   Compiling unicase v2.9.0
   Compiling quick-error v1.2.3
   Compiling bech32 v0.8.1
   Compiling strsim v0.10.0
   Compiling vec_map v0.8.2
   Compiling os_str_bytes v2.4.0
   Compiling unsigned-varint v0.2.3
   Compiling unicode-segmentation v1.13.3
   Compiling bech32 v0.11.1
   Compiling httpdate v1.0.3
   Compiling async-iterator v2.3.0
   Compiling endian-type v0.1.2
   Compiling cfg-if v0.1.10
   Compiling numtoa v0.1.0
   Compiling net2 v0.2.39
   Compiling ckb-sdk v5.1.0
   Compiling termion v1.5.6
   Compiling radix_trie v0.2.1
   Compiling hyper v0.14.32
   Compiling bitcoin v0.33.0-alpha.0 (https://github.com/rust-bitcoin/rust-bitcoin?rev=436de8ef12ab371aab6e9f6fbfb098238b42657d#436de8ef)
   Compiling parity-multihash v0.1.3
   Compiling clap v3.0.0-beta.1
   Compiling jsonrpc-server-utils v18.0.0
   Compiling ckb-cli v2.0.0 (/Users/.cargo/git/checkouts/ckb-cli-490787d2c61ea46c/ebfedb2)
   Compiling proc-macro-crate v0.1.5
   Compiling humantime v1.3.0
   Compiling scrypt v0.2.0
   Compiling chrono v0.4.45
   Compiling jsonrpc-client-transports v18.0.0
   Compiling aes-ctr v0.6.0
   Compiling dispatch2 v0.3.1
   Compiling tiny-keccak v1.5.0
   Compiling crossbeam-channel v0.5.17
   Compiling yaml-rust v0.4.5
   Compiling uuid v0.7.4
   Compiling regex v1.13.1
   Compiling parking_lot v0.12.5
   Compiling itertools v0.8.2
   Compiling fd-lock v4.0.4
   Compiling is-terminal v0.4.17
   Compiling utf8parse v0.2.2
   Compiling arrayref v0.3.9
   Compiling unicode-width v0.2.2
   Compiling data-encoding v2.11.1
   Compiling cassowary v0.3.0
   Compiling bs58 v0.2.5
   Compiling home v0.5.12
   Compiling parity-multiaddr v0.4.1
   Compiling rustyline v14.0.0
   Compiling tui v0.6.2
   Compiling console v0.15.11
   Compiling colored v1.9.4
   Compiling env_logger v0.6.2
   Compiling ckb-util v1.3.1
   Compiling serde_yaml v0.8.26
   Compiling ckb-channel v1.2.1
   Compiling ctrlc v3.5.2
   Compiling clap_generate v3.0.0-beta.1
   Compiling jsonrpc-core-client v18.0.0
   Compiling jsonrpc-http-server v18.0.0
   Compiling jsonrpc-derive v18.0.0
   Compiling ckb-cli-plugin-protocol v1.3.1 (/Users/.cargo/git/checkouts/ckb-cli-490787d2c61ea46c/ebfedb2/plugin-protocol)
   Compiling ipnetwork v0.14.0
   Compiling rustyline-derive v0.10.0
   Compiling dirs v1.0.5
   Compiling rpassword v3.0.2
   Compiling shell-words v0.1.0
   Compiling ansi_term v0.11.0
   Compiling dtoa v0.4.8
   Compiling ckb-signer v0.4.1 (/Users/.cargo/git/checkouts/ckb-cli-490787d2c61ea46c/ebfedb2/ckb-signer)
    Finished `release` profile [optimized] target(s) in 2m 22s
  Installing /Users/.cargo/bin/ckb-cli
   Installed package `ckb-cli v2.0.0 (https://github.com/nervosnetwork/ckb-cli.git#ebfedb28)` (executable `ckb-cli`)
   ```

After this experience i raised issue on ckb-cli github https://github.com/nervosnetwork/ckb-cli/issues/685
