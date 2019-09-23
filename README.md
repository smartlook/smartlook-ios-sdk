# Smartlook iOS SDK

The documentation for iOS SDK can be found at https://smartlook.github.io/docs/sdk/ios/

This repository serves as an issue tracker.

# Changelog
All notable changes to this project will be documented here.

## [1.2.1] - 2019-09-23
### Fixed
- bug when Smartlook crashed on iOS 10.x when some kinds of views (e.g., `UIAlertController`) were used in the app
- bug when Smartlook crashed when the app started w/out network connection
### Added
- support for custom timed events

## [1.2.0] - 2019-09-09
### Added
- support for custom navigation events
### Changed
- improved recording when there are Maps, SpriteKit, SceneKit or Metal views in UIKit app
### Fixed
- bug when `isRecording` returned `true` before `Smartlook.setup()`
- various smaller issues

## [1.1.0] - 2019-07-23
### Changed
- new much consistent version of API, the legacy API marked as deprecated, see documentation for details
- better snapshot handlings to improve CPU and battery efficiency
### Fixed
- various small errors

## [1.0.0] - 2019-05-21
### Added 
- Crashlytics support: URL of the latest recording made by Smartlook during or before the crash is added to crashreports
- Timed events: custom events can record their duration
- Form analytics: the length of editign focus to individual UI elements is explicitly recorded
- Pause/Resume recording, init Smartlook w/out to start recording later
- Optional framerate parameter in Smartlook initialization
### Fixed
- crashes in some complex scenarios where delegate methods to e.g., UITableView are implemented with inheritance hierarchy

## [0.1.12] - 2019-03-25
### Fixed
- Optimized sensitive views overlays with respect to the device rotation and CPU load.

## [0.1.11] - 2019-03-4
### Added
- Supporting selector event on all `UIControl` instances, including `UIDatePicker`, `UISegmentedControl`, `UISlider`, `UIStepper` and `UISwitch`
- `UIView` has two new properties for direct setting of their *sensitivity* handling: `slSensitive` (boolean flag) and `slOverlay` (overlay colour)
  - these properties are also accessible in Xcode Interface Builder

### Fixed
- Location of accessed UITabBarItems
- More accurate overlay of sensitive views

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
