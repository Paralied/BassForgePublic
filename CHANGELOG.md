# Changes

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
