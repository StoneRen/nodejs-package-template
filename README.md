# nodejs-package-template

## install

[degit](https://github.com/Rich-Harris/degit)

Get bare minimum nodejs workspace

```bash
npx degit github:StoneRen/nodejs-package-template
# or
git clone --depth=1 git@github.com:StoneRen/nodejs-package-template.git
```

## Branch

```bash
npx degit github:StoneRen/nodejs-package-template#[brach]

git clone -b [brach] git@github.com:StoneRen/nodejs-package-template.git
```

Branch list as below:

- vite
- vite_tailwind

## prepare

```bash
rm -rf **/package-lock.json
npm i --ws
npm init -w ./packages/[project name]
```
