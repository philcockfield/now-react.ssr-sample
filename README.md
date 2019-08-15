# Now Sample Debug Repo

Sample repo for debugging a build issue with now.

[Conversation on spectrum](https://spectrum.chat/zeit/now/securing-mongodb-altas~11523c5d-d17d-4cce-a3a6-e1f3d5195f0a).

## Setup

    yarn install
    now dev

![error](https://user-images.githubusercontent.com/185555/63076083-07460e80-bf88-11e9-8dfa-f71b3c552c78.png)

## Referenced Module

This repo initializes my `@platform/react.ssr` module, which is a small [micro](https://github.com/zeit/micro) service that serves data via `307` redirects from assets on S3.

This module can be [found here](https://github.com/uiharness/platform/tree/master/code/react.ssr).

None of the code running within the [micro](https://github.com/zeit/micro) service touches `fs`.
