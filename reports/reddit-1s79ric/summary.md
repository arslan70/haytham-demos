We ran a market analysis on macshot based on your [Reddit post](https://www.reddit.com/r/SideProject/comments/1s79ric/i_built_a_free_opensource_screenshot_screen/).
The short version: the timing is genuinely strong and there's a real gap, but distribution is the bottleneck, not features.

## What we found that you might not know

**Shottr's pricing shift created a time-limited window, and it's closing.**
Shottr went paid ($8-12) in late 2024, and Snagit moved to subscription-only in 2025.
Right now, developers are actively searching for free alternatives.
But this window fades as people either settle into Shottr's paid tier or land on something else.
The next 6-12 months are the highest-leverage period for capturing that cohort.
After that, the "I just lost my free tool" trigger dries up.

**Your PII auto-redaction feature is genuinely unique across every competitor we checked.**
CleanShot X, Shottr, Snagit, Flameshot, Kap: none of them offer it.
That said, it's unlikely to be an acquisition driver on its own because developers don't search for it proactively.
The pain only registers after a leak happens.
It's a strong retention and differentiation feature once someone discovers it, but probably not the thing that gets them to install.

**Flameshot, the most comparable open-source option, is broken on macOS.**
After their v13.0 update, it only captures the desktop wallpaper and ignores open windows (GitHub issues #4189, #4306).
They also went through a 3-year development hiatus.
The open-source macOS screenshot niche is effectively unoccupied right now.
That's good for you, but it also means the track record for sustained open-source screenshot tools on macOS is poor, which is something potential users will wonder about.

## The sharpest risk

Shottr at $8 might just be cheap enough that most people don't bother switching.
There's no verified data showing that Shottr's pricing change actually drove users to alternatives.
Eight dollars is below the threshold where most developers feel subscription fatigue.
If the pitch is "free alternative to a paid tool," it works best against CleanShot X at $29/year, not against Shottr at $8 one-time.
Positioning against CleanShot X specifically (rather than Shottr) might be the sharper angle.

## One thing to try

Post a "Show HN" with the PII redaction angle as the hook, not just "free screenshot tool."
Lead with the security angle because "free CleanShot X alternative" is generic, but "the screenshot tool that auto-redacts your API keys before you paste into Slack" is specific and sticky.

Working looks like: 100+ upvotes, 50+ comments, and 500+ GitHub stars within 48 hours.
Not working looks like: fewer than 30 upvotes and fewer than 100 stars.
This test costs nothing and tells you in one day whether the developer community cares enough about the gap to act on it.

---

Full report with competitive analysis, risk breakdown, and financial feasibility: [validation-report.md](validation-report.md)
