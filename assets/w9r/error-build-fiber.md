pnpm install
! Corepack is about to download https://registry.npmjs.org/pnpm/-/pnpm-10.28.2.tgz
? Do you want to continue? [Y/n] Y

Scope: all 13 workspace projects
Lockfile is up to date, resolution step is skipped
Packages: +564
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

   ╭───────────────────────────────────────────────╮
   │                                               │
   │     Update available! 10.28.2 → 12.10.1.      │
   │     Changelog: https://pnpm.io/v/12.10.1      │
   │   To update, run: corepack use pnpm@12.10.1   │
   │                                               │
   ╰───────────────────────────────────────────────╯

Downloading @nervosnetwork/fiber-js@0.9.0: 13.59 MB/13.59 MB, done
Downloading @biomejs/cli-darwin-arm64@2.3.14: 15.36 MB/15.36 MB, done
Progress: resolved 564, reused 111, downloaded 449, added 564, done
node_modules/.pnpm/better-sqlite3@12.6.2/node_modules/better-sqlite3: Running install script, failed in 20.3s
.../node_modules/better-sqlite3 install$ prebuild-install || node-gyp rebuild --release
│ prebuild-install warn install No prebuilt binaries found (target=26.7.0 runtime=node arch=arm64 l…
│ gyp info it worked if it ends with ok
│ gyp info using node-gyp@11.5.0
│ gyp info using node@26.7.0 | darwin | arm64
│ gyp info find Python using Python version 3.14.5 found at "/opt/homebrew/opt/python@3.14/bin/pyth…
│ gyp info spawn /opt/homebrew/opt/python@3.14/bin/python3.14
│ gyp info spawn args [
│ gyp info spawn args '/-/.cache/node/corepack/v1/pnpm/10.28.2/dist/node_modules/node-gy…
│ gyp info spawn args 'binding.gyp',
│ gyp info spawn args '-f',
│ gyp info spawn args 'make',
│ gyp info spawn args '-I',
│ gyp info spawn args '/-/Development/github/personal/web3/fiber-pay/node_modules/.pnpm/…
│ gyp info spawn args '-I',
│ gyp info spawn args '/-/.cache/node/corepack/v1/pnpm/10.28.2/dist/node_modules/node-gy…
│ gyp info spawn args '-I',
│ gyp info spawn args '/-/Library/Caches/node-gyp/26.7.0/include/node/common.gypi',
│ gyp info spawn args '-Dlibrary=shared_library',
│ gyp info spawn args '-Dvisibility=default',
│ gyp info spawn args '-Dnode_root_dir=/-/Library/Caches/node-gyp/26.7.0',
│ gyp info spawn args '-Dnode_gyp_dir=/-/.cache/node/corepack/v1/pnpm/10.28.2/dist/node_…
│ gyp info spawn args '-Dnode_lib_file=/-/Library/Caches/node-gyp/26.7.0/<(target_arch)/…
│ gyp info spawn args '-Dmodule_root_dir=/-/Development/github/personal/web3/fiber-pay/n…
│ gyp info spawn args '-Dnode_engine=v8',
│ gyp info spawn args '--depth=.',
│ gyp info spawn args '--no-parallel',
│ gyp info spawn args '--generator-output',
│ gyp info spawn args 'build',
│ gyp info spawn args '-Goutput_dir=.'
│ gyp info spawn args ]
│ gyp info spawn make
│ gyp info spawn args [ 'BUILDTYPE=Release', '-C', 'build' ]
│ make: Entering directory '/-/Development/github/personal/web3/fiber-pay/node_modules/.…
│   TOUCH ba23eeee118cd63e16015df367567cb043fed872.intermediate
│   ACTION deps_sqlite3_gyp_locate_sqlite3_target_copy_builtin_sqlite3 ba23eeee118cd63e16015df36756…
│   TOUCH Release/obj.target/deps/locate_sqlite3.stamp
│   CC(target) Release/obj.target/sqlite3/gen/sqlite3/sqlite3.o
│   LIBTOOL-STATIC Release/sqlite3.a
│   CXX(target) Release/obj.target/better_sqlite3/src/better_sqlite3.o
│ In file included from ../src/better_sqlite3.cpp:34:
│ ../src/addon.cpp:36:3: warning: 'Value' is deprecated: Use the version with the type tag. [-Wdepr…
│    36 |                 OnlyAddon->SqliteError.Reset(OnlyIsolate, SqliteError);
│       |                 ^
│ ../src/util/macros.cpp:17:71: note: expanded from macro 'OnlyAddon'
│    17 | #define OnlyAddon static_cast<Addon*>(info.Data().As<v8::External>()->Value())
│       |                                                                       ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8-external.h:54:3: note: 'Value' has b…
│    54 |   V8_DEPRECATED("Use the version with the type tag.")
│       |   ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8config.h:615:35: note: expanded from …
│   615 | # define V8_DEPRECATED(message) [[deprecated(message)]]
│       |                                   ^
│ In file included from ../src/better_sqlite3.cpp:43:
│ ../src/objects/backup.cpp:46:2: warning: 'Value' is deprecated: Use the version with the type tag…
│    46 |         UseAddon;
│       |         ^
│ ../src/util/macros.cpp:20:33: note: expanded from macro 'UseAddon'
│    20 | #define UseAddon Addon* addon = OnlyAddon
│       |                                 ^
│ ../src/util/macros.cpp:17:71: note: expanded from macro 'OnlyAddon'
│    17 | #define OnlyAddon static_cast<Addon*>(info.Data().As<v8::External>()->Value())
│       |                                                                       ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8-external.h:54:3: note: 'Value' has b…
│    54 |   V8_DEPRECATED("Use the version with the type tag.")
│       |   ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8config.h:615:35: note: expanded from …
│   615 | # define V8_DEPRECATED(message) [[deprecated(message)]]
│       |                                   ^
│ In file included from ../src/better_sqlite3.cpp:44:
│ ../src/objects/statement.cpp:72:2: warning: 'Value' is deprecated: Use the version with the type …
│    72 |         UseAddon;
│       |         ^
│ ../src/util/macros.cpp:20:33: note: expanded from macro 'UseAddon'
│    20 | #define UseAddon Addon* addon = OnlyAddon
│       |                                 ^
│ ../src/util/macros.cpp:17:71: note: expanded from macro 'OnlyAddon'
│    17 | #define OnlyAddon static_cast<Addon*>(info.Data().As<v8::External>()->Value())
│       |                                                                       ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8-external.h:54:3: note: 'Value' has b…
│    54 |   V8_DEPRECATED("Use the version with the type tag.")
│       |   ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8config.h:615:35: note: expanded from …
│   615 | # define V8_DEPRECATED(message) [[deprecated(message)]]
│       |                                   ^
│ In file included from ../src/better_sqlite3.cpp:44:
│ ../src/objects/statement.cpp:229:2: warning: 'Value' is deprecated: Use the version with the type…
│   229 |         UseAddon;
│       |         ^
│ ../src/util/macros.cpp:20:33: note: expanded from macro 'UseAddon'
│    20 | #define UseAddon Addon* addon = OnlyAddon
│       |                                 ^
│ ../src/util/macros.cpp:17:71: note: expanded from macro 'OnlyAddon'
│    17 | #define OnlyAddon static_cast<Addon*>(info.Data().As<v8::External>()->Value())
│       |                                                                       ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8-external.h:54:3: note: 'Value' has b…
│    54 |   V8_DEPRECATED("Use the version with the type tag.")
│       |   ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8config.h:615:35: note: expanded from …
│   615 | # define V8_DEPRECATED(message) [[deprecated(message)]]
│       |                                   ^
│ In file included from ../src/better_sqlite3.cpp:44:
│ ../src/objects/statement.cpp:381:43: error: no member named 'This' in 'v8::PropertyCallbackInfo<v…
│   381 |         Statement* stmt = Unwrap<Statement>(info.This());
│       |                                             ~~~~ ^
│ In file included from ../src/better_sqlite3.cpp:45:
│ ../src/objects/database.cpp:155:2: warning: 'Value' is deprecated: Use the version with the type …
│   155 |         UseAddon;
│       |         ^
│ ../src/util/macros.cpp:20:33: note: expanded from macro 'UseAddon'
│    20 | #define UseAddon Addon* addon = OnlyAddon
│       |                                 ^
│ ../src/util/macros.cpp:17:71: note: expanded from macro 'OnlyAddon'
│    17 | #define OnlyAddon static_cast<Addon*>(info.Data().As<v8::External>()->Value())
│       |                                                                       ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8-external.h:54:3: note: 'Value' has b…
│    54 |   V8_DEPRECATED("Use the version with the type tag.")
│       |   ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8config.h:615:35: note: expanded from …
│   615 | # define V8_DEPRECATED(message) [[deprecated(message)]]
│       |                                   ^
│ In file included from ../src/better_sqlite3.cpp:45:
│ ../src/objects/database.cpp:203:2: warning: 'Value' is deprecated: Use the version with the type …
│   203 |         UseAddon;
│       |         ^
│ ../src/util/macros.cpp:20:33: note: expanded from macro 'UseAddon'
│    20 | #define UseAddon Addon* addon = OnlyAddon
│       |                                 ^
│ ../src/util/macros.cpp:17:71: note: expanded from macro 'OnlyAddon'
│    17 | #define OnlyAddon static_cast<Addon*>(info.Data().As<v8::External>()->Value())
│       |                                                                       ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8-external.h:54:3: note: 'Value' has b…
│    54 |   V8_DEPRECATED("Use the version with the type tag.")
│       |   ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8config.h:615:35: note: expanded from …
│   615 | # define V8_DEPRECATED(message) [[deprecated(message)]]
│       |                                   ^
│ In file included from ../src/better_sqlite3.cpp:45:
│ ../src/objects/database.cpp:261:2: warning: 'Value' is deprecated: Use the version with the type …
│   261 |         UseAddon;
│       |         ^
│ ../src/util/macros.cpp:20:33: note: expanded from macro 'UseAddon'
│    20 | #define UseAddon Addon* addon = OnlyAddon
│       |                                 ^
│ ../src/util/macros.cpp:17:71: note: expanded from macro 'OnlyAddon'
│    17 | #define OnlyAddon static_cast<Addon*>(info.Data().As<v8::External>()->Value())
│       |                                                                       ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8-external.h:54:3: note: 'Value' has b…
│    54 |   V8_DEPRECATED("Use the version with the type tag.")
│       |   ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8config.h:615:35: note: expanded from …
│   615 | # define V8_DEPRECATED(message) [[deprecated(message)]]
│       |                                   ^
│ In file included from ../src/better_sqlite3.cpp:45:
│ ../src/objects/database.cpp:411:50: error: no member named 'This' in 'v8::PropertyCallbackInfo<v8…
│   411 |         info.GetReturnValue().Set(Unwrap<Database>(info.This())->open);
│       |                                                    ~~~~ ^
│ ../src/objects/database.cpp:415:39: error: no member named 'This' in 'v8::PropertyCallbackInfo<v8…
│   415 |         Database* db = Unwrap<Database>(info.This());
│       |                                         ~~~~ ^
│ In file included from ../src/better_sqlite3.cpp:46:
│ ../src/objects/statement-iterator.cpp:79:2: warning: 'Value' is deprecated: Use the version with …
│    79 |         UseAddon;
│       |         ^
│ ../src/util/macros.cpp:20:33: note: expanded from macro 'UseAddon'
│    20 | #define UseAddon Addon* addon = OnlyAddon
│       |                                 ^
│ ../src/util/macros.cpp:17:71: note: expanded from macro 'OnlyAddon'
│    17 | #define OnlyAddon static_cast<Addon*>(info.Data().As<v8::External>()->Value())
│       |                                                                       ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8-external.h:54:3: note: 'Value' has b…
│    54 |   V8_DEPRECATED("Use the version with the type tag.")
│       |   ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8config.h:615:35: note: expanded from …
│   615 | # define V8_DEPRECATED(message) [[deprecated(message)]]
│       |                                   ^
│ ../src/better_sqlite3.cpp:48:1: warning: cast from 'void (*)(v8::Local<v8::Object>, v8::Local<v8:…
│    48 | NODE_MODULE_INIT(/* exports, context */) {
│       | ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
│ /-/Library/Caches/node-gyp/26.7.0/include/node/node.h:1377:3: note: expanded from macr…
│  1377 |   NODE_MODULE_CONTEXT_AWARE(NODE_GYP_MODULE_NAME,                     \
│       |   ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
│  1378 |                             NODE_MODULE_INITIALIZER)                  \
│       |                             ~~~~~~~~~~~~~~~~~~~~~~~~
│ /-/Library/Caches/node-gyp/26.7.0/include/node/node.h:1346:3: note: expanded from macr…
│  1346 |   NODE_MODULE_CONTEXT_AWARE_X(modname, regfunc, NULL, 0)
│       |   ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
│ /-/Library/Caches/node-gyp/26.7.0/include/node/node.h:1328:7: note: expanded from macr…
│  1328 |       (node::addon_context_register_func) (regfunc),                  \
│       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
│ ../src/better_sqlite3.cpp:60:47: warning: 'New' is deprecated: Use the version with the type tag.…
│    60 |         v8::Local<v8::External> data = v8::External::New(isolate, addon);
│       |                                                      ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8-external.h:31:3: note: 'New' has bee…
│    31 |   V8_DEPRECATED("Use the version with the type tag.")
│       |   ^
│ /-/Library/Caches/node-gyp/26.7.0/include/node/v8config.h:615:35: note: expanded from …
│   615 | # define V8_DEPRECATED(message) [[deprecated(message)]]
│       |                                   ^
│ 10 warnings and 3 errors generated.
│ make: *** [better_sqlite3.target.mk:136: Release/obj.target/better_sqlite3/src/better_sqlite3.o] …
│ rm ba23eeee118cd63e16015df367567cb043fed872.intermediate
│ make: Leaving directory '/-/Development/github/personal/web3/fiber-pay/node_modules/.p…
│ gyp ERR! build error
│ gyp ERR! stack Error: `make` failed with exit code: 2
│ gyp ERR! stack at ChildProcess.<anonymous> (/-/.cache/node/corepack/v1/pnpm/10.28.2/di…
│ gyp ERR! System Darwin 25.5.0
│ gyp ERR! command "/opt/homebrew/Cellar/node/26.7.0/bin/node" "/-/.cache/node/corepack/…
│ gyp ERR! cwd /-/Development/github/personal/web3/fiber-pay/node_modules/.pnpm/better-s…
│ gyp ERR! node -v v26.7.0
│ gyp ERR! node-gyp -v v11.5.0
│ gyp ERR! not ok
└─ Failed in 20.3s at /-/Development/github/personal/web3/fiber-pay/node_modules/.pnpm/better-sqlite3@12.6.2/node_modules/better-sqlite3
 ELIFECYCLE  Command failed with exit code 1.
