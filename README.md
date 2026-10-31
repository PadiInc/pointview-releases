# Pointview apps

Download the latest from **Releases** (right-hand side of this page).

| Computer | File |
|---|---|
| Mac with Apple silicon (M1 and later) | `Pointview-…-arm64.dmg` |
| Mac with Intel | `Pointview-…-x64.dmg` |
| Windows | `Pointview-Setup-….exe` |
| Linux | `Pointview-…-x86_64.flatpak` or `Pointview-…-x86_64.AppImage` |

Not sure which Mac? Apple menu → About This Mac: "Chip: Apple M…" is Apple silicon; "Processor: Intel" is Intel.

## Mac

The Mac app isn't signed by Apple yet, so the first time needs one extra step.

1. Open the `.dmg` and drag Pointview into Applications.
2. Open Pointview. The Mac says it can't verify it. Click **Done** (not Move to Trash).
3. Open **System Settings → Privacy & Security**, scroll down, and click **Open Anyway** next to Pointview. Enter your password.
4. Open Pointview again and click **Open Anyway**.

After that it opens normally.

## Windows

The Windows app is signed by Padi, Inc.

1. Run `Pointview-Setup-….exe` and follow the installer.
2. Pointview then opens from the Start menu.

Windows may still be cautious while the signature is new. If you see "Windows protected your PC", check that the publisher is Padi, Inc., then click **More info** and **Run anyway**.

## Linux

No warning to get past. Install the Flatpak from your software centre, or mark the AppImage as allowed to run (`chmod +x`) and open it.

To update the Flatpak, remove the old one first, then open the new file. Your account and keys stay:

```
flatpak uninstall --user com.padi.pointview
```

(Use `--system` instead of `--user` if it was installed for everyone; `flatpak list` shows which.)
