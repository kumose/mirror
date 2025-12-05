# Component Mirror Repository

This repository is a mirror of pre-built components, following the standard layout for easy distribution and management.

## Directory Structure
- **components/**: Flat directories for each component (e.g., server-a/), containing binary packages (*.tar.gz) and manifest files (*.manifest.json).
- **versions/**: Version index files grouped by component name prefix (e.g., s-/ for server-* components). Each component has a dedicated JSON file with version details.
- **index.json**: Root index of all available components and their latest versions.
- **baseline.json**: Baseline configuration for mirror synchronization and compatibility.
- **LICENSE**: License information for the mirror and components.

## Usage
1. Clone this repository (use Git LFS to pull large binary files: \'git lfs install && git clone <repo-url>\').
2. Browse components in the \'components/\' directory by name, version, OS, and architecture.
3. Check version details in the \'versions/\' directory for specific components.

## Component Filename Format
All components follow the standard filename format:
<ComponentName>-<Version>-<OS>-<Arch>.<Suffix>
Example: server-a-1-3-1-linux-amd64.tar.gz (binary) / server-a-1-3-1-linux-amd64.manifest.json (manifest)

## License
This mirror and its components are licensed under the GNU Affero General Public License v3.0 (see LICENSE file).
