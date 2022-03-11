## Convert this to DOC

## from Markdown
https://daringfireball.net/projects/markdown/syntax#header

https://garrettgman.github.io/rmarkdown/authoring_pandoc_markdown.html

### to PDF
    pandoc README.md -s -o README.pdf

### to HTML
    pandoc README.md -s -o README.html

## References
[^1]: [Creating a snap](https://snapcraft.io/docs/creating-a-snap).

[^2]: https://snapcraft.io/docs/snapcraft-overview

[^3]: https://snapcraft.io/docs/creating-a-snap

[^4]: https://snapcraft.io/docs/snapcraft-format

[^5]: https://snapcraft.io/docs/snapcraft-top-level-metadata

[^6]: https://snapcraft.io/docs/snapcraft-parts-metadata

[^7]: https://snapcraft.io/docs/snapcraft-app-and-service-metadata

[^8]: https://snapcraft.io/docs/snapcraft-yaml-reference

[^9]: [Iterating over a build](https://snapcraft.io/docs/iterating-over-a-build)

[^10]: https://snapcraft.io/docs/build-options "Build Options"

* Base snaps

> https://snapcraft.io/docs/base-snaps[^11]

[^11]: [Base snaps](https://snapcraft.io/docs/base-snaps).

[^12]: [Convenient ways to fix up missing library](http://forum.snapcraft.io/t/convenient-ways-to-fix-up-the-missing-library-stage-packages-prompt/9163)

https://snapcraft.io/docs/snapcraft-advanced-grammar

Identifying missing packages, Build and staging dependencies
https://snapcraft.io/docs/build-and-staging-dependencies#heading--missing

Build on LXD
https://snapcraft.io/docs/build-on-lxd

Build and Publish Snap Packages using Snapcraft on CircleCI 
https://circleci.com/docs/2.0/build-publish-snap-packages/?utm_source=google&utm_medium=sem&utm_campaign=sem-google-dg--latam-en-dsa-maxConv-auth-brand&utm_term=g_-_c__dsa_&utm_content=&gclid=CjwKCAiA9tyQBhAIEiwA6tdCrKaLoKtZVTDQDUXZ3Y0HrxqR7t3Sl_LoqeWu43wsGOWoP0i0rqT3ERoCAekQAvD_BwE

## Interesting points
> * Use the try argument with both the snapcraft and snap commands.
> $ snapcraft try builds the snap and copies its prime directory to the current working directory on the host system - outside of any build environment container.
[^9]

> * snapcraft --use-lxd
> Builds the snap using LXD, rather than Multipass. This can potentially reduce resource usage, especially from a VM. Set SNAPCRAFT_BUILD_ENVIRONMENT=lxd to use LXD by default. Requires LXD
[^10]

> * bare: an empty base that’s useful with fully statically linked snaps and when testing
> [^11]

> * Convenient ways to fix-up the missing library stage-packages prompt[^12]


## Commands
 $ snapcraft --debug # builds the snap package with debug level log
 $ snapcraft clean # cleansup space from snap package builds

## Reading now
https://snapcraft.io/docs/creating-a-snap

## Done
	- added vscode as dependency with 'stage-snap' entry in snapcraft.yaml
	- fixed missing libs with stage-packages and dpkg -S
	

## Working at
Clean build with
 $ snapcraft --debug


## TODO
 - install 
   - jdk 
   - mvn 
   - junit
   - quarkus
   - vscode-plugins
     - https://stackoverflow.com/questions/34286515/how-to-install-visual-studio-code-extensions-from-command-line
   - prometheus
   - mongodb
   - mongodb client
 - install this snap on windows under wsl  
