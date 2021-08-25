# JTD

## Test regression between Jekyll versions v4.1.1..v4.2.0

### Requirements

- Jekyll versions 4.2.0 (and 4.1.1 for comparison) installed in the test environment.
- `just-the-docs` theme installed locally.
- `bash` or `sh` executables (*Optional*).

### Repro steps

- Clone this repository.
- Open two terminal windows, both with the clone destination as the *current directory*.
- In the first terminal window, run:
    ```
    bash _scripts/serve-4.1.1
    ```
- Preview served debug output at `http://localhost:4000/debug/`
- In the second terminal window, run:
    ```
    bash _scripts/serve-4.2.0
    ```
- Preview served debug output at `http://localhost:4001/debug/` in a new tab.
- Compare contents in the two tabs.
