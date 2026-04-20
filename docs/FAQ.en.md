# Dogdou FAQ

[Back to README](../README.md) | [中文常见问题](./FAQ.zh-CN.md) | [English Guide](./guide.en.md)

## What Is Audio Reuse?

On consumer editions of Windows, audio devices are typically limited to a single session at a time. The purpose of audio reuse is to allow multiple sessions to reuse the same audio device.

It is recommended to enable audio reuse once before starting a new session, and to use the audio restore action when you need to return audio ownership to its default state.

## What Does "Start With Shell" Mean?

If this option is enabled, the system will automatically start the default shell program when the session launches, usually `explorer.exe`. In this mode, the experience is broadly the same as using a normal desktop environment.

If this option is not enabled, the session starts without loading a shell, which means you enter an environment without a desktop. In that case, you can manually launch the programs you need through the create process feature.

This mode uses fewer system resources and is better suited for scenarios that do not require a full desktop interface.

## What Does the Create Process Feature Do?

The create process feature starts the specified program inside the selected session. The default command is usually `cmd.exe`, but it can be changed to another executable and can also include startup arguments.

Additional notes:

- The command path can use environment variables, for example `%windir%\system32\cmd.exe`
- If the command path contains spaces, it must be wrapped in quotes, for example `"%windir%\system32\cmd.exe"`

## Are There Limits on Sessions or Processes?

There is currently no hard limit on the number of sessions, but creating too many sessions may cause system resources to become constrained.

There is also no hard limit on the number of processes inside a session, but too many processes may increase resource pressure within that session.

In addition, processes created inside a session can access system resources, but whether that access succeeds still depends on the current user permissions and the system security policy.
