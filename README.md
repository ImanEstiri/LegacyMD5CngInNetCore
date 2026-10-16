# LegacyMD5CngInNetCore

A cross-platform compatibility library for legacy .NET applications that need MD5 hashing on modern .NET runtimes.

## 🛠️ Overview

`LegacyMD5CngInNetCore` aims to simplify the migration of legacy applications that rely on the `MD5Cng` API to modern .NET environments, including Linux, macOS, and Docker containers.

It provides an alternative approach to generating MD5 hashes on platforms where the Windows-specific `MD5Cng` implementation is unavailable, while helping preserve compatibility with existing hashing workflows.

## 🚀 Key Features

- **Cross-Platform Support:** Designed for Linux, macOS, and containerized environments.
- **Modern .NET Compatibility:** Intended for applications targeting modern .NET versions, including .NET 6, 7, and 8.
- **Legacy Integration:** Helps reduce changes when migrating applications that depend on the legacy `MD5Cng` API.
- **Native Cryptography Support:** Relies on the cryptographic capabilities available through the underlying .NET runtime and platform.

## 📦 Use Cases

- Migrating legacy applications from .NET Framework to modern .NET.
- Maintaining compatibility with systems that require MD5-based checksums.
- Supporting legacy integrations that depend on existing MD5 hashing behavior.
- Testing and debugging cross-platform applications that use MD5.

## ⚠️ Security Considerations

- **MD5 is cryptographically broken.** Do not use it for passwords, digital signatures, or security-sensitive integrity verification.
- **Not FIPS-compliant by default.** Using MD5 does not provide FIPS compliance, regardless of the underlying platform or implementation.
- **Compatibility is not guaranteed.** Verify hash outputs and platform behavior against your existing implementation before deploying to production.

## 🎯 Goal

Provide a practical migration path for legacy .NET applications that need to preserve MD5-based compatibility while moving to modern, cross-platform runtimes.
