# Changelog

All notable changes to Pushwoosh Unity SDK will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.12] - 2026-03-30

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

### Changes
- Fix duplicate GUID conflict between link.xml and PushwooshIOSDependencies.xml

## [1.0.11] - 2026-03-30

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

### Changes
- Fix packaging issues found by review
- Add meta file for link.xml

## [1.0.10] - 2026-03-30

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

### Changes
- Remove redundant link.xml from platform packages
- Move link.xml to core package (single file for all assemblies)
- Add link.xml to prevent IL2CPP code stripping

## [1.0.9] - 2026-03-30

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

### Changes
- Fix NSE: handle null ARCHS build property

## [1.0.8] - 2026-03-30

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

### Changes
- Fix NSE: support both UPM and .unitypackage paths

## [1.0.7] - 2026-03-30

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

### Changes
- Update README with Windows platform
- Add Windows (UWP/WSA) platform support
- Fix docs: remove metadata table, add Windows platform badge
- Rewrite documentation
- Restructure public GitHub repo to UPM layout
- Update internal README: clarify auto version bump
- Add internal README with release process and CI documentation

## [1.0.6] - 2026-03-30

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

## [1.0.5] - 2026-03-30

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

## [1.0.4] - 2026-03-30

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

## [1.0.3] - 2026-03-30

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

### Changes
- Add ANDROID_HOME to CI variables

## [1.0.2] - 2026-03-27

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

### Changes
- Use HTTPS for public SDK tag checks (no SSH key needed for read-only)

## [1.0.1] - 2026-03-27

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33

### Changes
- Fix changelog generation: use temp file instead of awk with newlines
- Fix all review issues: rename dirs to match package.json, add .meta files, update scripts
- Fix CocoaPods validation to use pod spec cat instead of CDN API
- Rename UPM packages to com.akidislab.* for testing
- Add verify stage (iOS/Android/packages), rename to upm-publish, add prerelease-check skill

## [1.0.0] - 2026-03-27

### Native SDK Updates
- Android SDK: 6.7.60
- iOS SDK: 7.0.33
