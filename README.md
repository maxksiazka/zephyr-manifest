# Zephyr manifest repository

This is my Zephyr manifest repository.
It contains the `west.yml` file that defines the Zephyr project and its dependencies.

It sets up a Zephyr workspace in a T3 topology, 
```
.
├── apps <--- User applications
├── boards <--- Out-of-tree boards
├── manifest <--- This is the manifest repository
│   ├── README.md
│   └── west.yml
├── modules <--- Out-of-tree modules
├── scripts <--- Out-of-tree scripts
└── zephyrproject <--- Zephyr project, and its imports
    ├── bootloader
    ├── doc
    ├── modules
    ├── tools
    └── zephyrproject
```

If you know how to make zephyr not generate inside its own `zephyrproject` directory, please let me know.
## How to use this repository

1. Choose a directory where you want to set up your Zephyr workspace.
2. Create a manifest repository by cloning this repository.
3. Initialize the Zephyr workspace using the `west` tool.
```bash
west init -l
```

