# Week 1 Report

**Week ending:** Aug 12, 2026

This week was mostly about getting my dev environment working and wrapping my head around how CKB actually thinks about state.

## What I learned

Coming from an ETH background, I expected CKB to feel similar, but it doesn't. CKB uses a **Cell model** instead of accounts — cells get created and destroyed with every transaction, and you pay for the storage you use (1 CKB = 1 byte, roughly). It's a different mental model but it clicked once I saw a transaction get built manually in the Academy exercises: you're literally consuming old cells and producing new ones.

I also went through **Intro to Script**, which is CKB's version of a smart contract. A Script is just a binary that runs in CKB-VM and returns 0 for success. There are two kinds — Lock Script (controls who can spend a cell) and Type Script (controls how a cell can change) — and they get executed differently depending on whether they're on an input or output. That distinction didn't make sense to me at first, but it's basically why the two are used for different things: Lock for ownership, Type for validation rules.

Finished **CKB Academy lessons 1 and 2**. Lesson 1 was mostly theory (cells, capacity, locks). Lesson 2 was hands-on — connect a wallet to testnet, then build a transfer transaction by hand: fill in cellDeps and inputs, generate the tx hash, sign it, serialize the witness, and broadcast. Ran into two errors along the way (see below), but got a transaction actually confirmed on testnet, which felt good.

On the `nckb` side, I got OffCKB running with a local devnet and deployed the `hello-world` contract. Also wrote/ran a test that sends a real transaction against the deployed contract on devnet instead of just mocking it, so I have actual proof the thing works, not just that it compiles.

## Challenges

- `offckb --help` doesn't cover everything, so figuring out the right flags took some trial and error (e.g. `offckb deploy` needs `-y` to skip an interactive prompt that isn't obvious from `--help`).
- First deploy attempt failed with "0 contracts / no binary to deploy" — turned out I forgot to run the build step first. Rookie mistake, fixed by building before deploying.
- Academy Lesson 2 threw two errors while building the manual transaction:
  - `cellDeps[0].depType must be either code or depGroup` — I had the wrong value in that field.
  - A signature validation failure (`error code 71`) when sending the tx — traced it to `witnesses[0]` having a double `0x` prefix from being serialized twice. Cleaned that up and the transaction went through.

## Screenshots

| | |
|---|---|
| ![1](assets/w1r/1.jpeg) | First deploy attempt failing — kept this one as a record of the mistake. |
| ![2](assets/w1r/2.png) | Local devnet healthy via CKB Node Monitor, fully synced. |
| ![3](assets/w1r/3.png) | `hello-world.devnet.test.ts` passing — real tx sent and verified on devnet. |
| ![4](assets/w1r/error-save-transaction.png) | The `depType` error from Academy Lesson 2. |
| ![5](assets/w1r/error-send-transaction.png) | The signature validation error, before I fixed the witness field. |

## Next steps

Moving on to the beginner exercises, starting with Transfer CKB.
