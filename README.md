#WindowBuilder Website Source

This project contains the source code for the WindowBuilder website

https://eclipse.dev/windowbuilder/

## Getting started

Clone the project with submodules and start a web server:

```bash
git clone --recurse-submodules https://github.com/eclipse-windowbuilder/windowbuilder-website-source.git
cd  windowbuilder-website-source
hugo server
```

### Update hugo-solstice-theme

The [hugo-solstice-theme](https://gitlab.eclipse.org/eclipsefdn/it/webdev/hugo-solstice-theme) was added to this project as a git submodule.

```bash
git submodule update --remote
```

For more information, please see git documentation on [submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules).

## How to build my project's website with Jenkins?

The preferred static website generator for Eclipse project websites is [Hugo](https://gohugo.io/). 

You should first put your Hugo sources in a dedicated Git repository, either at GitHub if your source code is already hosted at GitHub or at [gitlab.eclipse.org](https://gitlab.eclipse.org). If you don't have such a repository already, feel free to [open a request](https://gitlab.eclipse.org/eclipsefdn/helpdesk/-/issues/new), the Eclipse IT team will create one for you.

Note that each and every Eclipse project automatically gets a Git repository with `git.eclipse.org/www.eclipse.org/<project_name>` (see this [repository index](https://git.eclipse.org/r/plugins/gitiles/www.eclipse.org/) for complete list). This is not where you want to push your Hugo sources. This repository contains the webpages that are automatically and regularly pulled and published on the www.eclipse.org HTTP server. All the content from the master branch will eventually be available at the URL https://www.eclipse.org/<project_name>.

## Contributing

1. [Fork](https://docs.gitlab.com/ee/user/project/repository/forking_workflow.html) the [windowbuilder-website-source](https://github.com/eclipse-windowbuilder/windowbuilder-website-source) repository
2. Clone repository: `git clone --recurse-submodules https://github.com/eclipse-windowbuilder/windowbuilder-website-source.git`
3. Create your feature branch: `git checkout -b my-new-feature`
4. Commit your changes: `git commit -m 'Add some feature' -s`
5. Push feature branch: `git push origin my-new-feature`
6. Submit a pull request

### Declared Project Licenses

This program and the accompanying materials are made available under the terms
of the Eclipse Public License v. 2.0 which is available at
http://www.eclipse.org/legal/epl-2.0.

SPDX-License-Identifier: EPL-2.0

## Related projects

### [solstice-assets](https://gitlab.eclipse.org/eclipsefdn/it/webdev/solstice-assets)

Images, less and JavaScript files for the Eclipse Foundation look and feel.

### [hugo-solstice-theme](https://gitlab.eclipse.org/eclipsefdn/it/webdev/hugo-solstice-theme)

Hugo theme of the Eclipse Foundation look and feel. 

## Trademarks

* Eclipse® is a Trademark of the Eclipse Foundation, Inc.
* Eclipse Foundation is a Trademark of the Eclipse Foundation, Inc.

## Copyright and license

Copyright 2021 the [Eclipse Foundation, Inc.](https://www.eclipse.org) and the [windowbuilder-website-source](https://github.com/eclipse-windowbuilder/windowbuilder-website-source/graphs/contributors). Code released under the [Eclipse Public License Version 2.0 (EPL-2.0)](https://raw.githubusercontent.com/eclipse-windowbuilder/windowbuilder-website-source/master/LICENSE).
