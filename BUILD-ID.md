# LookAt 0.1.0 (.hmod) - build notes
Source: d3grando/lookat, commit f07818c (MIT), unchanged.
Blocks only: API 0.1 has no entity/health/harvest-tool support (those are in the native 0.2.x .hnmod).

Build on a PC:
  rustup target add wasm32-unknown-unknown
  cargo install --git https://github.com/horizon-rust/horizon cargo-horizon-mod
  cargo horizon-mod build        # -> target/horizon-mod/lookat.hmod

Build from a phone: create a GitHub repo, upload these files, open
Actions > "Build lookat.hmod" > Run workflow, then download the artifact.
(The workflow is untested.)
