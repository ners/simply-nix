# simply-nix

**simply-nix** is a GitHub Action that does two things:
- installs Nix in your GitHub CI runner
- (optional) cleans up unnecessary files in the GitHub CI environment to give more space to the Nix store

Why use it instead of other popular Nix actions? Because it is *very fast*, and frees up *a lot of space* for your builds.

It's also dead simple to use. Check it out:

## Usage

```yaml
steps:
  - uses: ners/simply-nix@main
    with:
      reclaim_space: true
```
That's it! You can now use Nix in your workflow. ✨

## Real-world examples

Here are some projects that use **simply-nix** in their CI:
- https://github.com/ners/trilby/blob/main/.github/workflows/ci.yml
- https://github.com/ners/syntax/blob/master/.github/workflows/ci.yml
- ... perhaps your own?
