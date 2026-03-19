## Service Worker Cache

After every edit to any file, increment the cache version number in `sw.js`:
`const CACHE = 'activity-picker-vN';`
Increment N by 1 from whatever the current value is. Do this even for small changes.

## Deployment
This is a GitHub Pages site. The production URL is sarahtrebatleder.github.io/bordem/.
Always test that the service worker and manifest paths are relative, not absolute.

## Data
Do not modify the Firestore data schema (the `list` array structure on user documents)
without explicitly being asked to. Schema changes can break existing user data.

## Layout
This is a PWA installed on iOS. Mobile layout is the primary experience.
Desktop layout is an enhancement. Never modify mobile styles as a side effect
of desktop changes.

## Scope
Make only the changes explicitly requested. Do not refactor, rename, or reorganize
code that isn't directly related to the task.
