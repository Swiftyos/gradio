# @gradio/file

## 0.1.3

### Patch Changes

- Updated dependencies [[`c57f1b75e`](https://github.com/gradio-app/gradio/commit/c57f1b75e272c76b0af4d6bd0c7f44743ff34f26), [`40de3d217`](https://github.com/gradio-app/gradio/commit/40de3d2178b61ebe424b6f6228f94c0c6f679bea), [`ea0e00b20`](https://github.com/gradio-app/gradio/commit/ea0e00b207b4b90a10e9d054c4202d4e705a29ba), [`75ddeb390`](https://github.com/gradio-app/gradio/commit/75ddeb390d665d4484667390a97442081b49a423)]:
  - @gradio/client@0.4.0
  - @gradio/upload@0.3.0

## 0.1.2

### Patch Changes

- Updated dependencies [[`afac0006`](https://github.com/gradio-app/gradio/commit/afac0006337ce2840cf497cd65691f2f60ee5912), [`26fef8c7`](https://github.com/gradio-app/gradio/commit/26fef8c7f85a006c7e25cdbed1792df19c512d02)]:
  - @gradio/statustracker@0.2.0
  - @gradio/client@0.3.1
  - @gradio/utils@0.1.1
  - @gradio/atoms@0.1.2
  - @gradio/upload@0.2.1

## 0.1.1

### Patch Changes

- Updated dependencies [[`119c8343`](https://github.com/gradio-app/gradio/commit/119c834331bfae60d4742c8f20e9cdecdd67e8c2), [`abf1c57d`](https://github.com/gradio-app/gradio/commit/abf1c57d7d85de0df233ee3b38aeb38b638477db), [`79d8f9d8`](https://github.com/gradio-app/gradio/commit/79d8f9d891901683c5a1b7486efb44eab2478c96)]:
  - @gradio/client@0.3.0
  - @gradio/icons@0.1.0
  - @gradio/utils@0.1.0
  - @gradio/upload@0.2.0
  - @gradio/atoms@0.1.1
  - @gradio/statustracker@0.1.1

## 0.1.0

### Highlights

#### Improve startup performance and markdown support ([#5279](https://github.com/gradio-app/gradio/pull/5279) [`fe057300`](https://github.com/gradio-app/gradio/commit/fe057300f0672c62dab9d9b4501054ac5d45a4ec))

##### Improved markdown support

We now have better support for markdown in `gr.Markdown` and `gr.Dataframe`. Including syntax highlighting and Github Flavoured Markdown. We also have more consistent markdown behaviour and styling.

##### Various performance improvements

These improvements will be particularly beneficial to large applications.

- Rather than attaching events manually, they are now delegated, leading to a significant performance improvement and addressing a performance regression introduced in a recent version of Gradio. App startup for large applications is now around twice as fast.
- Optimised the mounting of individual components, leading to a modest performance improvement during startup (~30%).
- Corrected an issue that was causing markdown to re-render infinitely.
- Ensured that the `gr.3DModel` does re-render prematurely.

Thanks [@pngwn](https://github.com/pngwn)!

### Features

- [#5215](https://github.com/gradio-app/gradio/pull/5215) [`fbdad78a`](https://github.com/gradio-app/gradio/commit/fbdad78af4c47454cbb570f88cc14bf4479bbceb) - Lazy load interactive or static variants of a component individually, rather than loading both variants regardless. This change will improve performance for many applications. Thanks [@pngwn](https://github.com/pngwn)!
- [#5216](https://github.com/gradio-app/gradio/pull/5216) [`4b58ea6d`](https://github.com/gradio-app/gradio/commit/4b58ea6d98e7a43b3f30d8a4cb6f379bc2eca6a8) - Update i18n tokens and locale files. Thanks [@hannahblair](https://github.com/hannahblair)!
- [#5221](https://github.com/gradio-app/gradio/pull/5221) [`f344592a`](https://github.com/gradio-app/gradio/commit/f344592aeb1658013235ded154107f72d86f24e7) - Allows setting a height to `gr.File` and improves the UI of the component. Thanks [@abidlabs](https://github.com/abidlabs)!
- [#5265](https://github.com/gradio-app/gradio/pull/5265) [`06982212`](https://github.com/gradio-app/gradio/commit/06982212dfbd613853133d5d0eebd75577967027) - Removes scrollbar from File preview when not needed. Thanks [@abidlabs](https://github.com/abidlabs)!
- [#5264](https://github.com/gradio-app/gradio/pull/5264) [`46a2b600`](https://github.com/gradio-app/gradio/commit/46a2b600a7ff030a9ea1560b882b3bf3ad266bbc) - ensure translations for audio work correctly. Thanks [@hannahblair](https://github.com/hannahblair)!

### Fixes

- [#5253](https://github.com/gradio-app/gradio/pull/5253) [`ddac7e4d`](https://github.com/gradio-app/gradio/commit/ddac7e4d0f55c3bdc6c3e9a9e24588b2563e4049) - Ensure File component uploads files to the server. Thanks [@pngwn](https://github.com/pngwn)!
- [#5313](https://github.com/gradio-app/gradio/pull/5313) [`54bcb724`](https://github.com/gradio-app/gradio/commit/54bcb72417b2781ad9d7500ea0f89aa9d80f7d8f) - Restores missing part of bottom border on file component. Thanks [@abidlabs](https://github.com/abidlabs)!

## 0.0.3

### Patch Changes

- Updated dependencies [[`61129052`](https://github.com/gradio-app/gradio/commit/61129052ed1391a75c825c891d57fa0ad6c09fc8), [`667875b2`](https://github.com/gradio-app/gradio/commit/667875b2441753e74d25bd9d3c8adedd8ede11cd), [`67265a58`](https://github.com/gradio-app/gradio/commit/67265a58027ef1f9e4c0eb849a532f72eaebde48), [`8b4eb8ca`](https://github.com/gradio-app/gradio/commit/8b4eb8cac9ea07bde31b44e2006ca2b7b5f4de36)]:
  - @gradio/client@0.2.0
  - @gradio/upload@0.0.3

## 0.0.2

### Patch Changes

- Updated dependencies []:
  - @gradio/utils@0.0.2
  - @gradio/atoms@0.0.2
  - @gradio/upload@0.0.2
