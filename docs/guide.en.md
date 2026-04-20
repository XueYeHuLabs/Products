# Dogdou Guide

[Back to README](../README.md) | [Chinese Guide](./guide.zh-CN.md) | [English Changelog](./changelog.en.md)

## Installation

1. Download the installer from the repository `Releases` tab.
2. Run the installer as Administrator.
3. Files are copied into `%ProgramData%\Dogdou`.
4. The installer also registers the uninstall entry, driver, and `DogdouService`.

Notes:

- The installer is not stored in the repository tree
- The `.exe` and checksum files should be downloaded from the release page

![Install](./media/install.png)

## First Launch

1. Start `DogdouToolkit.exe` from the desktop shortcut or install directory.
2. The current primary sections are:
   - `Session`
   - `Credentials`
   - `About`
3. Create a credential before starting the first session.

## Create a Credential

1. Open the `Credentials` page.
2. Click `+ New`.
3. Create a credential entry for later session startup.

![Credentials Setup 1](./media/credentials-setup-1.png)
![Credentials Setup 2](./media/credentials-setup-2.png)
![Credentials Setup 3](./media/credentials-setup-3.png)

## Start a Session

1. Return to the `Session` page.
2. Select a credential in `Select Credential`.
3. Fill in width, height, and refresh rate.
4. Enable `Start with shell` if needed.
5. Click `Start Session`.

Real UI capture:

![Dogdou Toolkit Session Start 1](./media/start-session-setup-1.png)
![Dogdou Toolkit Session Start 2](./media/start-session-setup-2.png)
![Dogdou Toolkit Session Start 3](./media/start-session-setup-3.png)
![Dogdou Toolkit Session Start 4](./media/start-session-setup-4.png)
![Dogdou Toolkit Session Game Example](./media/local-linker-game-example.png)

## Create a Process and Link

1. Confirm the session appears in the session list.
2. Enter a program in `Command Line`, for example `cmd.exe`.
3. Set `Work Directory`, for example `%USERPROFILE%`.
4. Click `Create Process`.
5. Click `Link Session` to enter the environment.
6. For audio handling, use `Reuse Audio` before starting a new session, and use `Resume Audio` when you need to restore audio output.
