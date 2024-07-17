# tapestry-antora-site-poc-content

## About
Proof of concept of how the Tapestry website and documentation could be based on Antora.
Intended for futher discussion with the Tapestry team.

This repo exclusively contains the website and documentation sources.
See the [tapestry-antora-site-poc-builder](https://github.com/vjlamp/tapestry-antora-site-poc-builder) repo for how Antora is configured to build a static website from these sources.

## Why isn't this hosted in an official Apache repo?
We may convert it into one eventually.
To get started, this personal repo was a quick and easy for me to have a shared repo - essential for the intended Antora setup.

## Migration Strategy
Currently, the Tapestry website is generated from a Confluence Wiki hosted by the Apache Software Foundation.
In contrast, Antora works with Asciidoc sources.
The strategy is to migrate the content manually.
1. Copy the content from the current Tapestry website and paste it into the corresponding Asciidoc page.
2. Enhance the source by recreating (i.e. adding missing) typography and by adding `javadoc:` and `issue:` macros where appropriate.
3. Copy the Asciidoc page to the version branches.
4. For each version branch, remove content no longer, or not yet, relevant for that branch.

Using automated scripts to convert Confluence sources to Asciidoc sources could be of some use. However, the larger part of the work is to split up the version-specific parts across the branches. Probably not worth the time to develop scripts for that.

## Contributing
This is hosted on GitHub so please feel invited to send **pull requests**.
If you would, please follow the [One sentence per line](https://asciidoctor.org/docs/asciidoc-recommended-practices/#one-sentence-per-line) principle.

