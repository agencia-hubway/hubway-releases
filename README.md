# Hubway releases

Release zips and update manifests for Agência Hubway's WordPress plugins, Hubway MCP and Hubway Essentials. The plugins' source is private; what this repository holds is what every site running them already has.

Each plugin's `Update URI` header names its manifest, served by GitHub Pages:

- `https://agencia-hubway.github.io/hubway-releases/hubway-mcp.json`
- `https://agencia-hubway.github.io/hubway-releases/hubway-site-essentials.json`

WordPress reads the manifest on its usual update checks and offers the release it names, whose zip is an asset of this repository's release `<plugin>-<version>`. To install a plugin on a site for the first time, download its zip from [Releases](https://github.com/agencia-hubway/hubway-releases/releases) and upload it under Plugins → Add New → Upload Plugin.

Never edit a manifest by hand: Hubway MCP's `tools/publish-release.sh` creates the release and writes it.
