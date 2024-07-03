# my keeb
only have one mechanical keyboard right now, which is this one. may build more in the future, but happy so far. can build on Windows in WSL, or macOS with optional .envrc file

## build details
TBD

## qmk commands
build clangd database: `qmk generate-compilation-database -kb mode/m256wh -km mariolopjr`
build keeb: `qmk compile -kb mode/m256wh -km mariolopjr`

## update
Quick instructions in updating from upstream
```bash
git checkout main
git pull --rebase upstream main
git submodule update --init --recursive
git checkout keebs
git merge main
```

Then run qmk build command. May need to regenerate clangd database, dunno
