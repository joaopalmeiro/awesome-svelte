# Notes

- [pnpm](https://pnpm.io/):
  - Package manager (for Node.js).
  - The files inside `node_modules` are linked (symlinks) from a single [content-addressable storage](https://en.wikipedia.org/wiki/Content-addressable_storage) (all files are stored in a single place on disk). With npm or Yarn, if you have 10 projects using a dependency, you will have 10 copies of that dependency on disk (compared to 1 copy with pnpm).
  - Also, if you depend on different versions of the dependency, only the files that differ are added to the storage.
  - [Non-flat `node_modules` directory](https://pnpm.io/motivation#creating-a-non-flat-node_modules-directory) (strict).
  - Installation (macOS): `curl -f https://get.pnpm.io/v6.16.js | node - add --global pnpm`.
  - [Uninstall pnpm](https://pnpm.io/uninstall).
  - Commands:
    - `pnpm init` ([Implement `pnpm init` (instead of passing through to `npm init`)](https://github.com/pnpm/pnpm/issues/3505) open issue).
    - `pnpm --version`.
    - `pnpm install`.
    - `pnpm add <pkg>`.
    - `pnpm <cmd>`.
  - [What Is pnpm?](https://youtu.be/hiTmX2dW84E) by [LevelUpTuts](https://leveluptutorials.com/):
    - [VS Code theme](https://github.com/leveluptuts/level-up-vscode-theme).
    - [Render](https://render.com/) for hosting:
      - It supports pnpm.
      - [Deploy a Svelte Static Site](https://render.com/docs/deploy-svelte) page and [project template](https://github.com/render-examples/svelte).
