# Contribution guide

Trivadis welcomes contributions to this repository from anyone.

If you want to submit a pull request to fix a bug or improve an existing good practice, please open an issue first and link to that issue when you submit your pull request.

If you have any questions about a possible submission, feel free to open an issue too.

## Contributing to the Good Practice Guide

All contributors are expected to adhere to our [code of conduct](CODE_OF_CONDUCT.md).

Pull requests are made under ... to be defined

For pull requests to be accepted, the bottom of your commit message must have
the following line using your name and e-mail address.

```bash
Signed-off-by: Your Name <you@example.org>
```

This will be automatically added to pull requests if you using the `signoff`
parameter when committing your changes:

```bash
  git commit [--signoff|-S]
```

## Oracle product ownership and responsibility

For any new product content, *you must obtain internal Oracle approvals for the
distribution of this content prior to submitting a pull request*. If you are
unfamiliar with the approval process to submit code to an existing GitHub
repository, please contact the [Oracle Open Source team](mailto:opensource_ww_grp@oracle.com)
for details.

The GitHub user who submits the initial pull request to add a new product image
should add themselves to the [code owner](./CODEOWNERS) file in that same
request. This will flag the user as the owner of the content and any future pull
requests that affect the content will need to be approved by this user.

The code owner will also be assigned to any issues relating to their content.

You must ensure that you check the [issues](https://github.com/oracle/docker-images/issues)
on at least a weekly basis, though daily is preferred.

...

Contact [Stefan Oehrli](https://github.com/oehrlis) for more information.

### Pull request process

1. Fork this repository
1. Create a branch in your fork to implement the changes. We recommend using
the issue number as part of your branch name, e.g. `1234-fixes`
1. Ensure that any documentation is updated with the changes that are required
by your fix.
1. Ensure that any samples are updated if the base image has been changed.
1. Submit the pull request. *Do not leave the pull request blank*. Explain exactly
what your changes are meant to do and provide simple steps on how to validate
your changes. Ensure that you reference the issue you created as well.
We will assign the pull request to 1-2 people for review before it is merged.

## Golden Rules

We have some golden rules that all submitted *good practice* must adhere to.
These rules are provided by Trivadis Knowledge Management and may change at any time.

Most of these are targeted at Trivadis employees, but apply to anyone who submits
a pull request.

### Base *Good Practice* rules

1. Extend an existing *Good Practice* wherever possible rather than create new ones.
1. Follow the KISS principle. keep it simple, stupid
1. 

### Security-related rules

1. Do not hard-code any passwords or ssh keys.

### Documentation rules

1. No Oracle host or domain names should be included in any code or examples.
   If an example domain name is required, use `example.com`.
1. All documentation including `README.md` files needs to meet Oracle
   documentation standards. For content submitted by internal Oracle teams,
   it is recommended that your documentation team either write or at least
   review this content. Externally submitted documentation will be reviewed
   during the PR process.
1. Wherever possible, refer to "container images" or just "images" in all
   documentation, as well as in any script output.

### Guidelines and recommendations

The following are some guidelines that will not prevent an image from being
merged, but are generally frowned upon if breached.

* Always aim to produce the smallest possible image. This means using multi-stage
  builds with a final stage using the least amount of layers possible. Combine
  as much as possible within a single directive and be sure to remove any
  cache created by `dnf` or `yum` or other tools.
* Don't install all possible required RPMs, even if the product
  documentation says so. Some RPMs aren't applicable inside a container, e.g
  filesystem utilities (`btrfs-progs`, `ocfs2-tools`, `nfs-utils`).
* Don't install any interactive/user tools, e.g. things like `vim`, `less` or
  `man`. Debugging should be done prior to the image submission.
* Don't install `wget` as the base images already include `curl`.
* Always remember to run `rm -rf /var/cache/yum` or `dnf clean all` in the same
  `RUN` directive as any `yum` or `dnf` command so that the metadata is not
  stored in the layer.
* Always document any inputs (via `--build-arg` or `-e`) required by
  `docker build` or `docker run`. This documentation should also clearly state
  any defaults that are used if no input is provided.
* If a custom value must be provided by the end-user, the build or run should
  gracefully fail if that value is not provided.
