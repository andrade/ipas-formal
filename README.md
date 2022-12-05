Prove secrecy of session keys MK, SK in MA:

```
$ tamarin-prover ma.spthy --prove
...
==============================================================================
summary of summaries:

analyzed: ma.spthy

  processing time: 0.056243283s

  secrecy (all-traces): verified (434 steps)
  associate (exists-trace): verified (5 steps)
  flow (exists-trace): verified (27 steps)

==============================================================================
```

Prove secrecy of client encryption key K in sealing:

```
$ tamarin-prover sealing.spthy --prove
...
==============================================================================
summary of summaries:

analyzed: sealing.spthy

  processing time: 0.038918764s

  types (all-traces): verified (12 steps)
  flow (exists-trace): verified (8 steps)
  secrecy (all-traces): verified (9 steps)

==============================================================================
```

Prove secrecy of client encryption key K in unsealing:

```
$ tamarin-prover unsealing.spthy --prove
...
==============================================================================
summary of summaries:

analyzed: unsealing.spthy

  processing time: 0.038293403s

  types (all-traces): verified (12 steps)
  flow (exists-trace): verified (10 steps)
  secrecy (all-traces): verified (17 steps)

==============================================================================
```