# Nextflow lint results

- Generated: 2026-02-06T15:51:38.569681+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/sanger-tol/telomere/windows/main.nf:41:76`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      def jar_locations = ["${moduleDir}/resources/usr/bin/telomere.jar", "${projectDir}/bin/telomere.jar", task.ext.jar]
                                                                             ^^^^^^^^^^
  ```
