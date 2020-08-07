# dummy-meta

## Pre-Requisites

* Install [meta](https://github.com/mateodelnorte/meta#readme).
* Clone the current repository

## Usage

Before using initializing the meta project, the structure will look something like:

```bash
➜  tmp git:(master) ✗ tree .
.
└── dummy-meta
    └── README.md

1 directory, 1 file
➜  tmp git:(master) ✗
```

After running ``meta git update``, all of the other repositories required for the meta project will also be included.  For example:

```bash
➜  dummy-meta git:(master) tree .
.
├── README.md
└── meta_repos
    ├── dummy-sub-1
    │   └── README.md
    └── dummy-sub-2
        └── README.md

3 directories, 3 files
```
