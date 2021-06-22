# ~Sushiswap~ Sushi1COIN Swap SDK

In-depth documentation on this SDK is available at [uniswap.org](https://uniswap.org/docs/v2/SDK/getting-started/).

# Purpose of this SDK / repository

Wanting to keep as much the same as SushiSwap/Uniswap as possible, we found there was no way to do this and allow potential future upgrades, without implementing our own package. This way we can just expand on all that already exists, and make modifications as we see fit.

If all goes well, we will be able to continue to use new revisions of the SushiSwap SDK without having to modify this package. Provided the original SDK does not change drastically (Non backwards compatible application breaking code).

This can be very useful for anyone looking to launch a SushiSwap clone.

## Running tests

To run the tests, follow these steps. You must have at least node v10 and [yarn](https://yarnpkg.com/) installed.

First clone the repository:

```sh
git clone https://github.com/sushiswap/sushiswap-sdk.git
```

Move into the sushiswap-sdk working directory

```sh
cd sushiswap-sdk/
```

Install dependencies

```sh
yarn install
```

Run tests

```sh
yarn test
```

You should see output like the following:

```sh
yarn run v1.22.4
$ tsdx test
 PASS  test/constants.test.ts
 PASS  test/pair.test.ts
 PASS  test/fraction.test.ts
 PASS  test/miscellaneous.test.ts
 PASS  test/entities.test.ts
 PASS  test/trade.test.ts

Test Suites: 1 skipped, 6 passed, 6 of 7 total
Tests:       3 skipped, 82 passed, 85 total
Snapshots:   0 total
Time:        5.091s
Ran all test suites.
✨  Done in 6.61s.
```
