# How to use

The `enumerate-assemblies` subcommand is used to enumerate assemblies.

## Syntax

```bash
recsa enumerate-assemblies [OPTIONS] INPUT OUTPUT
```

### Positional Arguments
1. `INPUT`: Relative path to the input file.
2. `OUTPUT`: Relative path to the output file.

### Options
- `--wip-dir`, `-w`: Directory to store intermediate files.
- `--overwrite`, `-o`: Overwrite output file if it exists.
- `--verbose`, `-v`: Print verbose output.
- `--help`: Show this message and exit.

## Example

Directory structure before running the command:
```
/
└── input.yaml
```

Command:
```bash
recsa enumerate-assemblies input.yaml output.yaml
```

Directory structure after running the command:
```
/
├── input.yaml
└── output.yaml
```

Input and output files are as follows:

??? example "Input File"
    ``` yaml title="input.yaml"
    --8<-- "assets.h/input.yaml"
    ```

??? example "Output File"
    ``` yaml title="output.yaml"
    --8<-- "assets.h/output.yaml"
    ```

!!! note
    See [Input File](input.md) and [Output File](output.md) for more details.
