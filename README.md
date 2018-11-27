# advent-of-spec

Advent of Code puzzles checked with [speculative](https://github.com/slipset/speculative)

## Rationale

The initial purpose of this repo is to check
[speculative](https://github.com/slipset/speculative) specs for usage that was
not accounted for yet. As a bonus undefined usage of core functions
may be detected.

This repo can also be used as a general corpus of Clojure programs, like [coal-mine](https://github.com/mfikes/coal-mine). This is useful for regression testing compiler patches for Clojure and ClojureScript.

## Contribute

What's in it for you?
* Your Advent of Code solutions will be checked against others. This excludes the possibility that your solution only works for your specific input.
* You will be encouraged to write portable Clojure code: a solution that runs on the JVM via Clojure and on Node via ClojureScript.

What's in it for the Clojure community?
* You are helping advance the [speculative](https://github.com/slipset/speculative) project, a collection of core specs.
* You are helping to build a large Clojure corpus for various purposes (see [Rationale](#rationale)).

PRs welcome. Use the following template:

``` clojure
(ns aos.y20nn.dnn.you
  (:require
   [aos.y20nn.dnn.data :refer [input answer-1 answer-2]]
   [clojure.test :refer [deftest is testing]]))

(deftest part-1
  (is true))

(deftest part-2
  (is true))
```

Replace `20nn` and `dnn` with the correct year and day, and replace `you` with
your Github/BitBucket/etc. username.  Make sure the tests for your solution pass
with the `test-one` script.

## Run

Run all tests:

    script/test

Run one test:

    script/test-one aos.y2017.d01.borkdude
    
Run without instrumentation:

    UNSTRUMENT=true script/test
    UNSTRUMENT=true script/test-one aos.y2017.d01.borkdude
