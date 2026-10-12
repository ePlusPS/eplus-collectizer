# ePlus Collectizer

Collect network device configuration and operational information for an ePlus Digital Twin or your own network lab.

## Download v1.5.0

- [Download the Collectizer kit](https://github.com/ePlusPS/eplus-collectizer/releases/download/v1.5.0/ePlus-Collectizer-v1.5.0.zip)
- [Release notes](https://github.com/ePlusPS/eplus-collectizer/releases/tag/v1.5.0)
- [SHA256 checksum file](https://github.com/ePlusPS/eplus-collectizer/releases/download/v1.5.0/SHA256SUMS.txt)

Extract the ZIP and begin with `Instructions.pdf`. Download the named kit asset; GitHub's automatically generated source-code archives are repository snapshots.

ZIP SHA256: `464944a28b807703a978c297a8593385b92a8424ad3c1babeee9e932c2b75c46`

## Inside the kit

- Customer instructions in `Instructions.pdf`.
- Sixteen screen-logging and device-local command files covering Arista EOS; Cisco IOS XE, IOS XR and NX-OS; Juniper Junos Evolved; Nokia SR Linux; and Nokia SR OS Classic CLI and MD-CLI.
- Six local sanitizer binaries for Windows, macOS and Linux on x64/ARM64.

Command availability depends on the device, software release and enabled features. A collection profile does not imply Digital Twin runtime support for every software version; consult the guide for qualification details.

## Collect and review

1. Read the guide and choose the profile matching your NOS and CLI mode.
2. Enable terminal logging for screen collection, or retrieve the output file created by the device-local profile. Review the commands before running them; device-local collection may replace an existing collection file.
3. Keep one collection file per device and use distinct filenames.
4. Run the appropriate local sanitizer when required by your data-handling policy, then review its output before sharing.
5. Transfer collections through the intake method agreed with your ePlus team, or use them for your own lab.

Sanitization removes recognized credential patterns while preserving network-design information such as hostnames, addresses, interfaces and routing structure. It is not a topology anonymizer and cannot guarantee removal of every secret format.

The kit contains no customer collections, vendor NOS images or Digital Twin server software. Do not post device output or credentials in public GitHub issues. Contact your ePlus team with the NOS, model, version and rejected command when requesting help.
