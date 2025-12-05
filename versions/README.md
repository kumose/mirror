# Versions Directory

This directory stores version information for each managed component, with each component having its own subdirectory containing version metadata.

Each component's subdirectory contains JSON files (or structured data) based on the ComponentVersionList structure, which includes:

- **Version entries**: A collection of ComponentVersion objects, each representing a specific version of the component, with details such as:
  - git-tree: Git commit hash associated with the version (populated after pre-operation)
  - version: Version number (supports parallel versioning)
  - binary: Path to the package binary file
  - manifest: Path to the manifest file (describing package contents)
  - channel: Release channel (e.g., stable, beta, alpha)
  - timestamp: Release timestamp

These metadata files are used by the kmdo tool to track available versions, manage installations/updates, and ensure compatibility across component releases.