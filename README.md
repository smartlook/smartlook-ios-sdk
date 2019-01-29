# Smartlook iOS SDK

The documentation for iOS SDK can be found at https://smartlook.github.io/docs/sdk/ios/

This repository serves as an issue tracker.

# Changelog
All notable changes to this project will be documented here.

## [0.1.10] - 2019-01-29
### Changes
- Sensitive input views (UITextField, UITextView) are hidden by default now, i.e., overlay is opt-out, not opt-in now
### Fixed
- UserAgent properly set for Smartlook communication
- Fixed snapshots generating when app switches keyWindow


## [0.1.9] - 2019-01-15
### Added
- Multitouch events
- Keyboard show/hide events
### Fixed
- Removed conflicting Crashlytics framework
- Some further minor bug fixes and tweaks
