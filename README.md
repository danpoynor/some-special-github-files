# WIP Example Repo Containing Some Special GitHub Files

## Description

A collection of [GitHub](https://github.com) repo files that briefly explains their use.

## Usage

- Read through this READMEs [Files](#files) section to discover each of their uses.
- Investigate the Further Reading links to learn more about each file.
- Copy/paste from the examples as needed.
- If you find this repo interesting star it for future reference.

## Contributing workflow

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Use [markdownlint-cli](https://github.com/igorshubovych/markdownlint-cli) to check for common markdown style inconsistency.

Here’s how we suggest you go about proposing a change to this project:

1. [Fork this project](https://docs.github.com/en/get-started/quickstart/fork-a-repo) to your account.
2. [Create a branch](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository) for the change you intend to make.
3. Make your changes to your fork.
4. [Create a pull request](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) from your fork’s branch to our master branch.

Using the web-based interface to make changes is fine too, and will help you by automatically forking the project and prompting to send a pull request too.

## FAQ

<details>
  <summary>Are all these files necessary?</summary>

Nope. Just use what you need.

</details>

<details>
  <summary>When should I name the file ending in .md?</summary>

Only files that end in `.md` will be rendered using markdown. Whenever you want the file to be visually rendered using feature like headings, sections, lists, clickable links, bold, italic, ... you should use `.md`.

</details>

<details>
  <summary>What about Jekyll files?</summary>

Adding these is currently under consideration.

</details>

<details>
  <summary>Why are filenames in all caps?</summary>

To avoid confusion with other files and to make them more noticeable as being a special file.

</details>

---
---

## Files

---

### :page_facing_up: `.gitignore`

<details>
  <summary>Description</summary>

  You can create a .gitignore file in your repository's root directory to tell Git which files and directories to ignore when you make a commit. To share the ignore rules with other users who clone the repository, commit the .gitignore file in to your repository.

  GitHub maintains an official list of recommended .gitignore files for many popular operating systems, environments, and languages in the github/gitignore public repository. You can also use gitignore.io to create a .gitignore file for your operating system, programming language, or IDE. For more information, see "[github/gitignore](https://github.com/github/gitignore)" and the "[gitignore.io](https://www.gitignore.io/)" site.
  
</details>

<details>
<summary>File location in the repository</summary>

- root
- any subdirectory

</details>

<details>
<summary>Examples</summary>

```text
# Compiled source #
###################
*.com
*.class
*.dll
*.exe
*.o
*.so

# Packages #
############
# it's better to unpack these files and commit the raw source
# git has its own built in compression methods
*.7z
*.dmg
*.gz
*.iso
*.jar
*.rar
*.tar
*.zip

# OS generated files #
######################
.DS_Store
.DS_Store?
._*
.Spotlight-V100
.Trashes
ehthumbs.db
Thumbs.db

# Logs
logs
*.log
npm-debug.log*
yarn-debug.log*
yarn-error.log*
lerna-debug.log*
.pnpm-debug.log*

# keys
keys.js

databases
*.log
*.sql
*.sqlite

# Diagnostic reports (https://nodejs.org/api/report.html)
report.[0-9]*.[0-9]*.[0-9]*.[0-9]*.json

# Runtime data
pids
*.pid
*.seed
*.pid.lock

# Directory for instrumented libs generated by jscoverage/JSCover
lib-cov

# Coverage directory used by tools like istanbul
coverage
*.lcov

# nyc test coverage
.nyc_output

# Grunt intermediate storage (https://gruntjs.com/creating-plugins#storing-task-files)
.grunt

# Bower dependency directory (https://bower.io/)
bower_components

# node-waf configuration
.lock-wscript

# Compiled binary addons (https://nodejs.org/api/addons.html)
build/Release

# Dependency directories
node_modules/
jspm_packages/

# Snowpack dependency directory (https://snowpack.dev/)
web_modules/

# TypeScript cache
*.tsbuildinfo

# Optional npm cache directory
.npm

# Optional eslint cache
.eslintcache

# Microbundle cache
.rpt2_cache/
.rts2_cache_cjs/
.rts2_cache_es/
.rts2_cache_umd/

# Optional REPL history
.node_repl_history

# Output of 'npm pack'
*.tgz

# Yarn Integrity file
.yarn-integrity

# dotenv environment variables file
.env
.env.test
.env.production

# parcel-bundler cache (https://parceljs.org/)
.cache
.parcel-cache

# Next.js build output
.next
out

# Nuxt.js build / generate output
.nuxt
dist

# Gatsby files
.cache/
# Comment in the public line in if your project uses Gatsby and not Next.js
# https://nextjs.org/blog/next-9-1#public-directory-support
# public

# vuepress build output
.vuepress/dist

# Serverless directories
.serverless/

# FuseBox cache
.fusebox/

# DynamoDB Local files
.dynamodb/

# TernJS port file
.tern-port

# Stores VSCode versions used for testing VSCode extensions
.vscode-test

# yarn v2
.yarn/cache
.yarn/unplugged
.yarn/build-state.yml
.yarn/install-state.gz
.pnp.*
```

If you want to ignore a file that is already checked in, you must untrack the file before you add a rule to ignore it. From your terminal, untrack the file.

```shell
$ git rm --cached FILENAME
```

[GitHub Docs: Configuring ignored files for all repositories on your computer](https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files#configuring-ignored-files-for-all-repositories-on-your-computer)

You can also create a global .gitignore file to define a list of rules for ignoring files in every Git repository on your computer. For example, you might create the file at ~/.gitignore_global and add some rules to it.

Configure Git to use the exclude file ~/.gitignore_global for all Git repositories.

```shell
$ git config --global core.excludesfile ~/.gitignore_global
```

[GitHub Docs: Excluding local files without creating a .gitignore file](https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files#excluding-local-files-without-creating-a-gitignore-file)]

If you don't want to create a .gitignore file to share with others, you can create rules that are not committed with the repository. You can use this technique for locally-generated files that you don't expect other users to generate, such as files created by your editor.

Use your favorite text editor to open the file called .git/info/exclude within the root of your Git repository. Any rule you add here will not be checked in, and will only ignore files for your local repository.

1. Open Terminal.
2. Navigate to the location of your Git repository.
3. Using your favorite text editor, open the file *.git/info/exclude*.

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: Ignoring files](https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files)
- [git-scm.com/docs/gitignore](https://git-scm.com/docs/gitignore)

</details>

---

### :page_facing_up: `.nojekyll`

<details>
<summary>Description</summary>

GitHub Pages will use Jekyll to build your site by default. If you want to use a static site generator other than Jekyll, disable the Jekyll build process by creating an empty file called `.nojekyll` in the root of your publishing source, then follow your static site generator's instructions to build your site locally.

Notes

- Prevents GitHub Pages from ignoring files that begin with an underscore.
- GitHub Pages does not support server-side languages such as PHP, Ruby, or Python.

</details>

<details>
<summary>File location in the repository</summary>

- root

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: About GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages)

</details>

---

### :page_facing_up: `ACKNOWLEDGMENTS.md.md`

<details>
<summary>Description</summary>

TODO

</details>

<details>
<summary>Naming</summary>

TODO

</details>

<details>
<summary>File location in the repository</summary>

TODO

</details>

<details>
<summary>Examples</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

TODO

</details>

---

### :page_facing_up: `CHANGELOG.md`

<details>
<summary>Description</summary>

Notes

- Might also be named CHANGES, HISTORY, NEWS, RELEASES, VERSIONS, etc.

</details>

<details>
<summary>Naming</summary>

- CHANGELOG
- CHANGELOG.txt
- CHANGELOG.md

</details>

<details>
<summary>File location in the repository</summary>

TODO

</details>

<details>
<summary>Examples</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: About CITATION files](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/about-citation-files)

</details>

---

### :page_facing_up: `CITATION.cff`

<details>
<summary>Description</summary>

You can add a CITATION.cff file to the root of a repository to let others know how you would like them to cite your work. The citation file format is plain text with human- and machine-readable citation information.

</details>

<details>
<summary>File location in the repository</summary>

TODO

</details>

<details>
<summary>Examples</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: About CITATION files](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/about-citation-files)

</details>

---

### :page_facing_up: `CODEOWNERS`

<details>
<summary>Description</summary>

Repository administrators can define exactly which people and teams need to review projects using the CODEOWNERS file. This feature automatically assigns reviewers based on Code Owners when a pull request changes any owned files, using the same syntax as the .gitignore file.

Use the CODEOWNERS file to ensure that changes to specific areas of the codebase are always reviewed by those with the most expertise.

</details>

<details>
<summary>File location in the repository</summary>

- root
- docs/
- .github/

</details>

<details>
<summary>Examples</summary>

```text
# @global-owner1 and @global-owner2 will be requested for
# review when someone opens a pull request.
*       @global-owner1 @global-owner2

# When someone opens a pull request that only
# modifies JS files, only @js-owner and not the global
# owner(s) will be requested for a review.
*.js    @js-owner

# The `docs/*` pattern will match files like
# `docs/getting-started.md` but not further nested files like
# `docs/build-app/troubleshooting.md`.
docs/*  docs@example.com

# In this example, @octocat owns any file in the `/apps` 
# directory in the root of your repository except for the `/apps/github` 
# subdirectory, as its owners are left empty.
/apps/ @octocat
/apps/github

# In this example, any change inside the `/apps` directory
# will require approval from @doctocat or @octocat.
/apps/ @doctocat @octocat

# In this example, any change inside the `/apps` directory
# will require approval from a member of the @example-org/content team.
# If a member of @example-org/content opens a pull request 
# with a change inside the `/apps` directory, their approval is implicit.
# The team is still added as a reviewer but not a required reviewer.
# Anyone can approve the changes.
/apps/ @example-org/content-team
```

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: About code owners](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/about-code-owners)
- [GitHub Docs: Managing code review assignment for your team](https://docs.github.com/en/organizations/organizing-members-into-teams/managing-code-review-assignment-for-your-team)

</details>

---

### :page_facing_up: `CODE_OF_CONDUCT.md`

<details>
<summary>Description</summary>

A code of conduct defines standards for how to engage in a community. It signals an inclusive environment that respects all contributions. It also outlines procedures for addressing problems between members of your project's community. For more information on why a code of conduct defines standards and expectations for how to engage in a community, see the [Open Source Guide](https://opensource.guide/code-of-conduct/).

</details>

<details>
<summary>File location in the repository</summary>

TODO

</details>

<details>
<summary>Examples</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: Adding a code of conduct to your project](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-code-of-conduct-to-your-project)

</details>

---

### :page_facing_up: `CONTRIBUTING.md`

<details>
<summary>Description</summary>

To help your project contributors do good work, you can add a file with contribution guidelines to your project repository's root, `docs`, or `.github` folder. When someone opens a pull request or creates an issue, they will see a link to that file. The link to the contributing guidelines also appears on your repository's `contribute` page.

For the repository owner, contribution guidelines are a way to communicate how people should contribute.

For contributors, the guidelines help them verify that they're submitting well-formed pull requests and opening useful issues.

For both owners and contributors, contribution guidelines save time and hassle caused by improperly created pull requests or issues that have to be rejected and re-submitted.

</details>

<details>
<summary>File location in the repository</summary>

- root
- docs/
- .github/

</details>

<details>
<summary>Examples</summary>

- [github/docs Contributing to this repository](https://github.com/github/docs/blob/main/CONTRIBUTING.md)
- [github/docs/contributing/ Contributing to github/docs](https://github.com/github/docs/tree/main/contributing)

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: Setting guidelines for repository contributors](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors)
- [GitHub Docs: Encouraging helpful contributions to your project with labels](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/encouraging-helpful-contributions-to-your-project-with-labels)
- [GitHub Docs: About community management and moderation](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/about-community-management-and-moderation)
- [GitHub Docs: Setting up your project for healthy contributions](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions)
- [GitHub Docs: Encouraging helpful contributions to your project with labels](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/encouraging-helpful-contributions-to-your-project-with-labels)
- [GitHub Docs: Moderating comments and conversations](https://docs.github.com/en/communities/moderating-comments-and-conversations)
- [Open Source Guides: Building Welcoming Communities](https://opensource.guide/building-community/)

</details>

---

### :page_facing_up: `CONTRIBUTORS.md`

<details>
<summary>Description</summary>

TODO

</details>

<details>
<summary>Naming</summary>

TODO

</details>

<details>
<summary>File location in the repository</summary>

TODO

</details>

<details>
<summary>Examples</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

TODO

</details>

---
### :page_facing_up: `ISSUE_TEMPLATE.md`

<details>
<summary>Description</summary>

TODO

</details>

<details>
<summary>File location in the repository</summary>

TODO

</details>

<details>
<summary>Examples</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

TODO

</details>

---

### :page_facing_up: `LICENSE`

<details>
<summary>Description</summary>

You can include an open source license in your repository to make it easier for other people to contribute.

If you include a detectable license in your repository, people who visit your repository will see it at the top of the repository page.

Notes

- If you go to "Add file" dropdown in your repo to create a new file and start naming with "License", a button will appear to the right for you to select a license template.

</details>

<details>
<summary>Naming</summary>

- LICENSE (most common)
- ICENSE.md
- ...

</details>

<details>
<summary>File location in the repository</summary>

TODO

</details>

<details>
<summary>Examples</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: Adding a license to a repository](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository)
- [GitHub Docs: Licensing a repository](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/licensing-a-repository)

</details>

---

### :page_facing_up: `README.md`

<details>
<summary>Description</summary>

TODO

</details>

<details>
<summary>Naming</summary>

- README
- README.txt
- README.md (most common)
- ...

</details>

<details>
<summary>File location in the repository</summary>

- root

</details>

<details>
<summary>Examples</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: About READMEs](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/about-readmes)

</details>

---

### :page_facing_up: `SECURITY.md`

<details>
<summary>Description</summary>

TODO

</details>

<details>
<summary>File location in the repository</summary>

TODO

</details>

<details>
<summary>Examples</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: Adding a security policy to your repository](https://docs.github.com/en/code-security/getting-started/adding-a-security-policy-to-your-repository)
- [GitHub Docs: Creating a default community health file](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

</details>

---

### :page_facing_up: `SUPPORT.md`

<details>
<summary>Description</summary>

TODO

</details>

<details>
<summary>File location in the repository</summary>

TODO

</details>

<details>
<summary>Examples</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: Adding support resources to your project](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-support-resources-to-your-project)
- [GitHub Docs: Creating a default community health file](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

</details>

---

### :open_file_folder: `.github/`

<details>
<summary>Description</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

TODO

</details>

---

### :page_facing_up: `.github/FUNDING.yml`

<details>
<summary>Description</summary>

FUNDING file displays a sponsor button in your repository to increase the visibility of funding options for your open source project.

</details>

<details>
<summary>File location in the repository</summary>

Automatically generated at `.github/FUNDING.yml`

</details>

<details>
<summary>Examples</summary>

```text
github: [octocat, surftocat]
patreon: octocat
tidelift: npm/octo-package
custom: ["https://www.paypal.me/octocat", octocat.com]
```

</details>

<details>
<summary>Further reading</summary>

- [GitHub Docs: Displaying a sponsor button in your repository](https://docs.github.com/en/github/administering-a-repository/managing-repository-settings/displaying-a-sponsor-button-in-your-repository)

</details>

---

### :open_file_folder: `.github/ISSUE_TEMPLATE/`

<details>
<summary>Description</summary>

Issue templates and their configuration file must be in a folder called `.github/ISSUE_TEMPLATE`

</details>

<details>
<summary>Further reading</summary>

TODO

</details>

---

### :page_facing_up: `.github/ISSUE_TEMPLATE/bug_report.md`

<details>
<summary>Description</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

TODO

</details>

---

### :page_facing_up: `.github/ISSUE_TEMPLATE/feature_request.md`

<details>
<summary>Description</summary>

TODO

</details>

<details>
<summary>Further reading</summary>

TODO

</details>
