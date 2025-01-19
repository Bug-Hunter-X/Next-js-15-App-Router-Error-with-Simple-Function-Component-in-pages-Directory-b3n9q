## Next.js 15 App Router Error with Simple Function Component in pages Directory

This repository demonstrates a bug in Next.js 15's App Router.  A simple function component in the `pages` directory throws an error when using the app router, even without any dynamic routes or other advanced features.

**Bug:**
When using the app router, a basic function component in the `pages` directory (e.g., `pages/index.js`) might throw an error that is not helpful in resolving the issue.

**Steps to reproduce:**
1. Create a new Next.js 15 app.
2. Replace the contents of `pages/index.js` with the code provided in `bug.js`.
3. Start the development server and observe the error.

**Solution:**
The error can be resolved by moving the function component to a different directory outside the `pages` directory (e.g., `app/page.js`) and using the app directory structure.  This works because Next.js 15's App Router handles the routing differently than the pages directory in previous versions.

See `bugSolution.js` for the corrected code and approach.
