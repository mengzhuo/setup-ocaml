# lint-opam

Perform several quality checks on the opam file.

## Usage

### Example workflow

```yml
jobs:
  lint-opam:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@v3

      - name: Use OCaml 4.14.x
        uses: ocaml/setup-ocaml@v2
        with:
          ocaml-compiler: 4.14.x
          dune-cache: true

      - name: Lint opam
        uses: ocaml/setup-ocaml/lint-opam@v2
```

## Inputs

See [action.yml](./action.yml) for inputs.