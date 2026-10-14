# Changes

## 1.0.2

- Fix hidden startup window flags on the native launcher and Python handoff.
- Show a startup window with Restart startup, Cancel, and Open log.
- Treat mutex ownership correctly, including abandoned owners and retained
  handles after a process is killed.
- Supervise setup and its children until a visible studio confirms readiness;
  force-closing startup stops that unfinished process tree.
- Restore an existing or minimized studio when the app is reopened.
- Recover only verified invisible Bass Forge 1.0.0/1.0.1 installer processes;
  unrelated PowerShell and Python applications are left alone.
- Use a versioned installed launcher so an older locked EXE cannot block repair.
- Record studio startup stages and native crash details in startup.log.
- Exercise real Windows EXE launch, visibility, setup handoff, and forced-stop
  recovery in CI, alongside the existing installer and audio tests.

## 1.0.1

- Visible six-stage first-launch setup with live activity, download progress,
  elapsed time, completed steps, and copyable error details.
- Reliable native installer process handling preserves exit codes, including
  fast silent successes, and drains standard output and error concurrently.
- Check for updates in the studio and Settings. Fetches updates from the
  public GitHub repository, verifies the download, prompts to save, and waits
  for the studio to close before starting setup.
- Reuses installed dependencies and model caches during updates.

## 1.0.0

- Initial native bass studio, YouTube and file import, local AI separation,
  two-stem editor, custom bass effects, graphic EQ, projects and audio export.
