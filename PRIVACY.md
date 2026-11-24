# Kira Connect Privacy Policy

Effective: November 24, 2026

This policy covers **Kira Connect**: the `kira-connect` command-line tool and
native messaging host, and the Kira Connect browser extension for Microsoft
Edge and Firefox (together, "Kira Connect"). It is developed by
[@miketweaver](https://github.com/miketweaver) ("we", "us").

## The short version

Kira Connect does not collect, store, sell or share your personal
information. It has no accounts, no servers, no analytics, no telemetry, no
crash reporting and no advertising. Everything it does happens on your own
computer, between your browser and programs you run.

## What we collect

Nothing. We do not operate any server that Kira Connect talks to, so no
data about you, your browsing or your use of Kira Connect ever reaches us.

## What Kira Connect handles on your computer

Kira Connect lets programs on your computer read from, and act in, websites
you are signed in to, using your own browser session. To do that it handles
the following, **only on your device**:

- **Responses from approved websites.** When a program asks, the extension
  fetches an approved URL, reads text from an approved page, or performs
  approved actions (such as typing and clicking) in a browser tab. Only
  websites listed in the approval list shipped with each release can be
  reached, and only after you grant the browser permission for them.
- **Passing results to local programs.** Results go from the extension to the
  Kira Connect native host over the browser's native messaging channel, and
  from there to the requesting program over a Unix socket in your home
  directory that only your user account can open.
- **What you approve.** When a website change needs your confirmation,
  the extension shows you what will be sent or done, in a window on your
  screen.

Response bodies and page text are held in memory, limited in size, and
discarded when the request finishes. Kira Connect does not write them to
disk, keep a history, or cache them.

Kira Connect keeps a few local files to work: a copy of its own program and
a lock file in `~/.kira-connect`, and a registration file in your browser's
native messaging folder. These contain no personal information.

## Cookies and sign-ins

Kira Connect never reads, copies or exports your cookies, passwords or
session tokens. Requests are made by your browser itself, which attaches
your existing sign-in the same way it would if you visited the site. The
extension does not request the browser's `cookies` permission.

## Browser permissions

The extension asks for:

- `nativeMessaging`, to talk to the Kira Connect program on your computer.
- `scripting`, to read text from, and act in, only the tabs it opens itself
  on approved websites.
- Optional access to specific websites, which you grant or refuse in the
  browser when you click **Connect**. Only websites in the approval list are
  ever requested.

It does not ask for access to your browsing history or to your other tabs.
In Firefox, the add-on declares that it collects no data.

## Other programs on your computer

While Kira Connect is connected, any program running under your user account
can ask it to read from or act in approved websites as you. You decide which
programs you run. If you use an AI assistant with Kira Connect, it can see
whatever it reads through Kira Connect, under that assistant's own terms
and privacy policy.

## Websites you use

The websites Kira Connect reaches for you (for example Google Chat) receive
requests from your browser just as they would if you used them yourself.
Their own privacy policies apply to that activity.

## Downloading and updates

Kira Connect is distributed through GitHub and a Homebrew tap. GitHub and
Homebrew may log downloads and other activity under their own privacy
policies. Kira Connect itself does not check for updates or contact any
server.

## Children

Kira Connect is a developer tool and is not directed at children under 13.
It collects no information from anyone, including children.

## Changes

Changes to this policy are published as commits to
[miketweaver/kira-policies](https://github.com/miketweaver/kira-policies),
with an updated effective date above. If Kira Connect ever starts handling
data differently, this policy will be updated before that release.

## Contact

Questions about this policy: open an issue at
<https://github.com/miketweaver/kira-policies/issues>.
