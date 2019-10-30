# Command

```bash
lw-commit [-s scheme-name] ([-d device-id] | [-dn device-name]) [-m 'commit message']
```

## Options

- **-s** (scheme name): This option specify the scheme for run the test. Default `Lively-Release-QA`.

Device id (-d) or device name (-dn) is **required** to run unit tests:
  - **-d** : Device id (UUID).
    ```bash
    lw-commit -d "47917784-F1C0-4413-B35A-EE7171517CE4"
    ```
  - **-dn** : Device name.
    ```bash
    lw-commit -dn "Jovani's iPhone"
    ```
*To show current devices:*
```bash
instruments -s devices
```
- **-m** : If this option is set, the tracked changes will be commited.
