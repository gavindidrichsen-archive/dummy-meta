# dummy-meta

## Pre-Requisites

* Install [meta](https://github.com/mateodelnorte/meta#readme).
* Clone the current repository.

## Usage

Before initializing the current meta repository, the directory structure will look something like:

```bash
➜  dummy-meta git:(master) tree .
.
└── dummy-meta
    └── README.md

1 directory, 1 file
➜  tmp git:(master) ✗
```

However, after running ``meta git update``, which  all of the other repositories required for the meta project will also be included.  For example:

```bash
➜  dummy-meta git:(master) meta git update

*** the following repositories have been added to .meta but are not currently cloned locally:
*** {
  'meta_repos/dummy-sub-1': 'https://github.com/gavindidrichsen/dummy-sub-1.git',
  'meta_repos/dummy-sub-2': 'https://github.com/gavindidrichsen/dummy-sub-2.git'
}
*** type 'meta git update' to correct.

/Users/gavindidrichsen/Documents/@REFERENCE/git/meta/example/tmp/dummy-meta/meta_repos/dummy-sub-2:
Cloning into 'meta_repos/dummy-sub-2'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
/Users/gavindidrichsen/Documents/@REFERENCE/git/meta/example/tmp/dummy-meta/meta_repos/dummy-sub-2 ✓

/Users/gavindidrichsen/Documents/@REFERENCE/git/meta/example/tmp/dummy-meta/meta_repos/dummy-sub-1:
Cloning into 'meta_repos/dummy-sub-1'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
/Users/gavindidrichsen/Documents/@REFERENCE/git/meta/example/tmp/dummy-meta/meta_repos/dummy-sub-1 ✓
➜  dummy-meta git:(master)
```

So that the new directory structure will look something like this:

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
