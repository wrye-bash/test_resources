Wrye Bash Testing Resources
=========

A repository housing binary blobs used for testing Wrye Bash.

The folder names are pretty self-explanatory. `saves` houses save files and
cosaves, with subfolders for each game. The same goes for `bsas`, etc.

All files need to have a `.meta` file accompanying them. Meta files tell Wrye
Bash's test suite what information it should *expect* to extract from the file,
so that it can raise errors when the extracted information differs. They are
[TOML](https://github.com/toml-lang/toml) files with the same name as the file
they belong to, but with a `.meta` extension appended after the original file's
extension. For example, `autosave.nvse` would need a `autosave.nvse.meta` file.

Each subfolder contains another README.md, which explains the syntax of the
`.meta` files expected in that subfolder.

## Contributing
You are more than welcome to contribute resources, we can always use more
test cases!
Please make sure you understand and accept the [license](LICENSE) of this
repository, in particular that by submitting a resource for inclusion here,
you are basically committing *that version* of the file to the public domain.
So be sure that
 1. You own the files you want to submit, and
 2. You're okay with licensing them under the aforementioned license
before submitting anything.

Once you are ready, [create a fork](https://help.github.com/en/github/getting-started-with-github/fork-a-repo)
and add the files you want to submit. Then you just have to
[create a pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request),
and wait for a maintainer to merge it, or respond to any changes they request.
