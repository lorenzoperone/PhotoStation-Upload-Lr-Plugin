# Bug Report: Shared Albums Issue in Photo StatLr

Hi there!

I'm experiencing a problem when publishing a collection using the Photo StatLr plugin. On the first attempt, an internal error prevents the photos from being published. If I try again, the photos are uploaded successfully.

## Steps to Reproduce

1. Set up the plugin and the publish service (see screenshots in the debug folder, no sensitive data included).
2. Add photos to the published collection.
3. Click "Publish" to start the upload: internal error occurs.
4. Click "Publish" again: photos are published correctly.

## Expected Result

Photos should be published successfully on the first attempt, without any errors.

## Actual Result

On the first attempt, the collection update remains active for a long time (even with just two photos), and the upload actually fails. On the second attempt, the photos are published as expected.

## Error Message / Screenshots

Main error message:

```
15:18:35, ERROR: That does it, I'm leaving! Internal error: '[string "PSPhotosAPI.lua"]:604: attempt to index field '?' (a nil value)'
```

Full log and screenshots are available in the debug folder.

## Software Versions

- Photo StatLr Plugin: 7.5.1.20251214
- Adobe Lightroom Classic: 14.5
- Synology Photos/Photo Station: (please specify version if needed)
- Operating System: MacBook Pro M3 Pro OSX 26.2.0.25C56

## Additional Notes

This bug only occurs on the first publish attempt after setup. On the second try, everything works fine. Full log and screenshots are available in the debug folder.

Thanks for your help and for your great work on the plugin!
