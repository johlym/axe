# auls-papertrail

With the advent of ULS ([1](https://developer.apple.com/reference/os/logging) [2](http://devstreaming.apple.com/videos/wwdc/2016/721wh2etddp4ghxhpcg/721/721_unified_logging_and_activity_tracing.pdf) [3](https://developer.apple.com/videos/play/wwdc2016/721/)), application developers are now free to totally stop logging to syslog built into macOS. This is great for them, bad if getting logs to an external logging service like Papertrail is still on the agenda.

The goal of this code is to capture logs from Apple's Unified Logging System and send them to Papertrail. It's hacky and can probably be done more efficiently, but Apple has chosen to go the way of `journald` with their own twist.
