# Contributing 💕

Important things to know and general guidelines for contributions.  We also recommend that you have a look at our [code of conduct](https://github.com/miamatriarx/miamatriarx/blob/main/code_of_conduct.md) and that you understand our purpose and mission, our goals and objectives and that the contribution you make is in alignment with what we're working for.

## Contribution

- If you have any issues with software you can report it by creating a new [issue](https://github.com/miamatriarx/miamatriarx/issues).
- You can have a look at the [project](https://github.com/miamatriarx/miamatriarx/projects) page to see the current roadmap and things we're working on and you're welcome to make a [pull request](https://github.com/miamatriarx/miamatriarx/pulls).  If you do then fork the repository and create a pull request from the fork.
- If you'd like to contribute something that's not software you can get in [contact](https://github.com/miamatriarx/miamatriarx/blob/main/support.md).
- You can contribute by [funding](https://github.com/miamatriarx/miamatriarx/blob/main/readme.md) us.

## Legal

- All software created by Mia Matriarx or by the Matriarx brand are free and open source software ([FOSS](https://en.wikipedia.org/wiki/Free_and_open-source_software)) under the [MIT](https://github.com/miamatriarx/miamatriarx/blob/main/license.md) license.
- Any contribution made to software owned by Mia Matriarx or the Matriarx brand, or to any Matriarx community, falls under [MIT](https://github.com/miamatriarx/miamatriarx/blob/main/license.md) and in doing so you void all claims to any intellectual property or copyright without any exceptions.
- Developer Certificate of Origin ([DCO](https://en.wikipedia.org/wiki/Developer_Certificate_of_Origin)) is enforced on all repositories in order to verify that you have agreed to our terms.
- For more information have a look at [contributing](https://github.com/miamatriarx/miamatriarx/blob/main/contributing.md).

## DCO

- [Create a new GPG key](https://docsmiamatriarx.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key).
- [Add the GPG key to your GitHub account](https://docsmiamatriarx.com/en/authentication/managing-commit-signature-verification/adding-a-gpg-key-to-your-github-account).
- Have a look at [how to sign your commits](https://docsmiamatriarx.com/en/authentication/managing-commit-signature-verification/signing-commits) using your GPG key.
- After you've set it up you can use `git commit -S -am "message"` in order to create a signed and verified commit.

## Semantic Versioning & Conventional Commits

We use semantic versioning with conventional commits which are used to automatically generate the version, changelog and release notes.  If you contribute code make sure you follow our convention, otherwise it will be rejected.

### Semantic Versioning

The version will be automatically generated from commits and tags.

### Conventional Commits

We use conventional commits in order to automatically generate the changelog and release notes and to make it easier to debug.

#### Commit

- When making a commit do so using `type(scope): description` as the format in order to specifcy the type of commit, the scope, whether or not it's a breaking change and the description.
- Use the directory that is the primary focus of your update as the scope.
- If the commit includes a breaking change then include `!` using `type(scope)!: description` as the format to specify that it changes existing code in a backwards incompatible way.
- Only use lowercase.

#### Example

`git commit -S -am "feature(module)!: a new module feature"`

- This shows that the commit is a new feature.
- It shows that the update is primarily scoped to the module directory.
- It shows that it contains a breaking change.
- It's lowercase'.

#### Types

- feature - A completely new feature.
- update - An update to an existing feature.
- patch - A relatively small update to a module or component.
- security - An update specifically related to security.
- performance - An update specifically related to performance.
- config - An update that changes any configurations.
- build - An update that changes the build.
- ci - An update related to continuous integration.
- platform - A platform specific update.
- fix - A bug or hot fix.
- deprecate - A feature is being deprecated.
- remove - A feature has been removed.
- revert - A rollback.
- task - A relatively insignificant yet necessary chore.
- refactor - Code refactoring.
- polish - Code formatting or styling.
- documentation - An update to the documentation.

#### Merging

We use a linear commit history in order to generate the changelogs and release notes and to make it easier to debug, so use rebase or squash merge in order to keep the history clean.  For almost every use case you should be using rebase instead of squashing in order to preserve the commit history and to properly reflect changes in the generated changelog.  However there are some things to keep in mind.

- Only use rebase if the commits on your local branch have never been pushed to remote.  If you pushed those commits to remote, rebasing it can be a potentially destructive action and then you should squash it instead.
- Each commit should have a meaningful and tangible update or change, if you've made a bunch of commits with silly messages like "fix typo" then you should squash it.  Don't include meaningless commits in the commit history.
