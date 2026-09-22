Result on Rust Contracts

cargo test -- --nocapture
    Finished `test` profile [unoptimized + debuginfo] target(s) in 3.17s
     Running unittests src/lib.rs (target/debug/deps/hello_world_rs-84c2f1eb6a41f318)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/main.rs (target/debug/deps/hello_world_rs-bb23182b0a4cecb4)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/mulham-133a04884a5c49a1)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/main.rs (target/debug/deps/mulham-34424ab58a558b92)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/tests-77d4be237882a9f4)

running 2 tests
[contract debug] This is a sample contract!
consume cycles: 7328
test tests::test_hello_world_rs ... ok
[contract debug] Args Len: 1
[contract debug] Args Data: [2a]
consume cycles: 18128
test tests::test_mulham ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests hello_world_rs

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests mulham

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
