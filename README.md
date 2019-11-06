# Command

```bash
lw-push [-s scheme-name] ([-d device-id] | [-dn device-name]) [-m 'commit message']
```

## Options

- **-s** (scheme name): This option specify the scheme for run the test. Default `Lively-Release-QA`.
- **-m** : If this option is set, the tracked changes will be commited.

Device id (-d) **or** device name (-dn) is **required** to run unit tests:
- **-d** : Device id (UUID).
    ```bash
    lw-push -d "47917784-F1C0-4413-B35A-EE7171517CE4"
    ```
- **-dn** : Device name.
    ```bash
    lw-push -dn "Jovani's iPhone"
    ```

## Notes
To show available devices, run:
```bash
instruments -s devices
```
## Install
Open `.bash_profile`, which will be located at `/Users/_TheUser_/.bash_profile`, and add this line to the file. If `.bash_profile` doesn't exist, create it.
```bash
export PATH=$PATH:/Users/_TheUser_/My/File/Folder
```
Add permissions
```bash
chmod u+x lw-push
```
Now, run the command
```bash
lw-push
```