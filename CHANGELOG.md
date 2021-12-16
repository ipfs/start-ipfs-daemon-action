# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Added
- `wait-for-addrs` input that controls whether the action waits for addresses to be assigned to the daemon

## [1.0.0] - 2021-12-14
### Added
- action that calls `ipfs daemon` with provided args and waits for `Daemon is ready` on stdout
- maximum socket receive buffer size override on Linux runners
