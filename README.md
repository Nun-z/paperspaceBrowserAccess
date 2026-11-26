# paperspaceBrowserAccess

A single web page for controlling a [Paperspace](https://www.paperspace.com/) machine. It has buttons to start, shut down, and restart the machine, and it shows the machine's current state (off, starting, ready, etc.), refreshing every few seconds. Nobody using the page needs a Paperspace login.

## Use cases
- Control your own VM from any device with a browser, without signing in to the Paperspace console.
- Give a client a link so they can power their VM on and off without being given your account details.

## Setup
1. In the Paperspace console, create a team API key. The page talks to the Paperspace v1 API (`api.paperspace.com/v1`), which replaced the Core API when it was retired in July 2024.
2. Open `index.html` and paste your machine ID and API key into the `CONFIG` block near the top of the script.
3. Host `index.html` on any web server or static hosting service.

If you want to make the page source harder to read, you can run it through an HTML obfuscator such as https://www.wmtips.com/tools/html-obfuscator/.

## License
[MIT](LICENSE)
