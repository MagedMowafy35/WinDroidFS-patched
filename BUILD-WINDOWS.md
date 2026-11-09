# Build patched WinDroidFS for Windows 10/11 x64

This source tree includes a GitHub Actions workflow at `.github/workflows/build-windows.yml`.

1. Create a GitHub fork of this repository and upload/commit this patched source tree to it (preserve the `.github/workflows` directory).
2. Open the fork's **Actions** tab and enable Actions if prompted.
3. Select **Build WinDroidFS (Windows)**, choose **Run workflow**, and run it on the default branch.
4. When the run completes successfully, download the `WinDroidFS-Windows-x64-patched` artifact. It contains `windroidfs.exe`, `windows-daemon.exe`, and `windroidfs-service.exe`.

The workflow compiles on `windows-2022` with the MSVC toolchain. The executables are x64 and intended for Windows 10/11 x64. This is a build workflow, not a prebuilt binary; the source patch has not been validated on a physical Windows 10 machine. Install WinFsp on the target PC as required by WinDroidFS.
