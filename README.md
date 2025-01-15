# A road-map for Bash

The GNU Bash project is one of the oldest open source software projects, having been under constant development since 1988.

Since 1993 it has been maintained by Chet Ramey.
We thank Chet for his tireless efforts, but some day, eventually, he will want to retire.

When that happens, it will take a team of people to replace him.
One of the functions of that team will be to maintain and publish a future changes roadmap, and that starts here.

## Participation Threshold

As a GNU project, Bash only accepts substantive contributions from persons who have signed an agreement that
assigns copyright to the Free Software Foundation on the legal basis of "work for hire".
This might not seem onerous, and actually has some important legal benefits when it comes to enforcing copyleft,
but the process takes days (or even weeks), and so
it stalls contributors right when they're most able and motivated to contribute.
Many are so de-motivated by this interruption that they simply give up and move on to other projects.

In contrast, projects on platforms like Github allow contributions to be licenced simply by committing a suitable
declaration to each project, or by attaching a default licence to your user account.

Whilst copyright enforcement is important, Bash in its current state is hardly a tempting target for people looking to
rip off open source software; other shell implementations such as Ash, Dash, or Zsh would be more appealing targets.

| Action Points |
|---|
| Review contributor licensing arrangements |
| Consider accepting unassigned contributions |
| Consider re-branding as a non-GNU project |

* Technically re-branding would be a project fork, but if the `bash.org` domain is moved, and all contributors move as well then that technical detail doesn't matter.

## Bug Tracker Reform

Bash is distributed with a secondary utility `bashbug` that is self-described as:
> Bashbug is used to send mail to the Bash maintainers for when Bash doesn't behave like you'd like, or expect.

The problem is that this description is _exactly_ true: it sends email, and does _not_ create a bug report.
As a result, the majority of issues are never recorded in the bug tracker.

The email sent by `bashbug` posts to a mailing list, which has transmogrified from 
a small list of actual maintainers into a "support" discussion list.

When tickets are (occasionally) created directly in the bug tracker, they do get posted to the list, but
replies on the list do not get attached to the bug ticket, meaning that they are completely wasted effort:
the person who created the ticket will never see them.

It is hard to escape the conclusion that the current arrangement of mailing list and separate bug tracker is
no longer fit for purpose. If we don't simply adopt Github, we should aim to achieve comparable functionality.

| Action Points |
|---|
| Implement bi-directional connection between the mailing list and the bug tracker |
| Consider migrating to a new platform |

* Bidirectional integration might be as simple as tagging mailing list posts with
  `Reply-To: 1234@bugtrack.bash.org`

## Project Management

### Division of responsibilities

#### Code review
#### Patch wrangler
#### Bug wrangler

