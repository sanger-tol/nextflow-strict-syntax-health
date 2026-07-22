# Nextflow lint results

- Generated: 2026-07-22T00:20:18.943985345Z
- Nextflow version: 26.07.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `conf/modules.config:136:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename ->
                        ^^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:175:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
