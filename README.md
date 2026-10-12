# Local Manifests for Tecno Pova 5 Pro 5G (`LH8n`)

Branch-specific local manifests for building various Android 16 (BP4A) and Android 17 (CP2A) custom ROMs on Crave.io, local workstations, or CI build environments.

---

## Usage

In your initialized ROM source root directory (`.repo` must exist):

```bash
# Clone the branch corresponding to your target ROM into .repo/local_manifests
git clone https://github.com/Swaggyxren/local_manifests.git -b <branch> .repo/local_manifests

# Sync repositories
/opt/crave/resync.sh
# Or standard repo sync:
# repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

---

## Available Branches

### Android 17 (CP2A)
| ROM / Target | Branch | Device Tree Branch | Vendor Tree Branch | Kernel Branch |
| :--- | :--- | :--- | :--- | :--- |
| **LineageOS 24.0** | `lineage-24.0` | `lineage-24.0` | `lineage-24.0` | `test` |
| **LineageOS 24.0 (Test)** | `lineage-24.0-test` | `lineage-24.0-test` | `lineage-24.0-test` | `test` |
| **RisingOS 17** | `rising-17` | `rising-17` | `lineage-24.0` | `test` |
| **YAAP 17** | `yaap-17` | `yaap-17` | `lineage-24.0` | `test` |
| **Project Infinity-X 17** | `infinity-17` | `infinity-17` | `lineage-24.0` | `test` |

### Android 16 (BP4A)
| ROM / Target | Branch | Device Tree Branch | Vendor Tree Branch | Kernel Branch |
| :--- | :--- | :--- | :--- | :--- |
| **LineageOS 23.2** | `lineage-23.2` | `lineage-23.2` | `lineage-23.2` | `test` |
| **LineageOS 23.2 (Test)** | `lineage-23.2-test` | `lineage-23.2-test` | `lineage-23.2-test` | `test` |
| **AxionOS 16.2** | `axion16.2` | `axion16.2` | `lineage-23.2` | `test` |
| **Lunaris AOSP 16.2** | `lunaris-16` | `lunaris-16` | `lineage-23.2` | `lunaris-16` |
