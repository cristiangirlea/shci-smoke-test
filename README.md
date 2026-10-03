# shci-smoke-test

The smoke target for [self-hosted-ci](https://github.com/cristiangirlea/self-hosted-ci) releases. Before
a private repository moves to a new tag, a runner set for this repository is brought up from a fresh
clone of that tag and this repository's one workflow must run on it (`make smoke TAG=<tag>`).

No runner exists between tests: the workflow only runs when the smoke test triggers it.
