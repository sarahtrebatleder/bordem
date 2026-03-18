## Service Worker Cache

After every edit to any file, increment the cache version number in `sw.js`:
`const CACHE = 'activity-picker-vN';`
Increment N by 1 from whatever the current value is. Do this even for small changes.
