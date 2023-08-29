[![test](https://github.com/deepset-ai/document-store/actions/workflows/test.yml/badge.svg)](https://github.com/deepset-ai/document-store/actions/workflows/test.yml)

# Example Store

This Github repository is a template that can be used to create custom document stores to extend
the new [Haystack](https://github.com/deepset-ai/haystack/) API available under the `preview`
package starting from version 1.15.

While the new API is still under active development, the new "Store" architecture is quite stable
and we are encouraging early adopters to contribute their custom document stores.

## Template features

By creating a new repo using this template, you'll get the following advantages:
- Ready-made code layout and scaffold to build a custom document store.
- Support for packaging and distributing the code through Python wheels using Hatch.
- Github workflow to build and upload a package when tagging the repo.
- Github workflow to run the tests on Pull Requests.

## How to use this repo

1. Create a new repository starting from this template. If you never used this feature before, you
   can find more details in [Github docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).
2. If possible, follow the convention `technology-haystack` for the name of the new repository,
   where `technology` can be for example the name of a vector database you're integrating.
3. Rename the package `src/example_store` to something more meaningful and adjust the Python
   import statements.
4. Edit `pyproject.toml` and replace any occurrence of `example_store` and `example-store` according
   to the name you chose in the previous steps.
5. Search the whole codebase for the string `#FIXME`, that's where you're supposed to change or add
   code specific for the database you're integrating.
6. If Apache 2.0 is not suitable for your needs, change the software license.

When your custom document store is ready and working, feel free to add it to the list of available
[Haystack Integrations](https://haystack.deepset.ai/integrations) by opening a Pull Request in
[this repo](https://github.com/deepset-ai/haystack-integrations).


## License

`example-store` is distributed under the terms of the [Apache-2.0](https://spdx.org/licenses/Apache-2.0.html) license.
