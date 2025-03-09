# Chrome Policies and Command Lines Switches
This is a collection of Chrome Policies and Command Lines Switches to reduce the exposure to annoyances.

See `chrome-policies.reg` from this repo.

Reference
- [Chrome Enterprise policy list](https://chromeenterprise.google/policies)
- [Enterprise policy URL pattern format](https://chromeenterprise.google/policies/url-patterns)
- [Chrome Command Line 1](https://peter.sh/experiments/chromium-command-line-switches)
- [Chrome Command Line 2](https://kapeli.com/cheat_sheets/Chromium_Command_Line_Switches.docset/Contents/Resources/Documents/index)
- [Chrome Command Line 3](https://gist.github.com/dodying/34ea4760a699b47825a766051f47d43b)
- [Chrome Command Line 4](https://ubuntu-mate.community/t/ultimate-disable-command-line-switches-for-opera-browser/20683)

## Command Line Options
While Policies are documented, it seems not easy to find an official reference of command line options. Some switches can be controlled by Policies, but some other are command line only, apparently.

These are my switches, in addition to the Policies REG file of this repo.

```
SETX G_CHROME_CMDLINE_OPT  "--disable-breakpad --disable-crash-reporter --disable-login-animations --disable-overlay-scrollbar --disable-smooth-scrolling --disable-speech-api --disable-suggestions-ui --safebrowsing-disable-download-protection --start-maximized --wm-window-animations-disabled"

chrome.exe %G_CHROME_CMDLINE_OPT% --profile-directory="%G_CHROME_YOUR_PROFILE%"

```