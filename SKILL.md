---
name: linkedin
description: Post updates, articles, and engage on LinkedIn via browser automation. Use when creating LinkedIn posts, checking notifications, viewing profile analytics, commenting, liking, or any LinkedIn interaction. Requires OpenClaw browser with an active LinkedIn session.
---

# LinkedIn Skill

Automate LinkedIn interactions via OpenClaw browser control. LinkedIn has no public posting API for individuals, so all actions use browser automation.

## Prerequisites

- OpenClaw browser profile `openclaw` logged into LinkedIn
- Always use `profile=openclaw` for browser actions

## Posting an Update

1. Navigate to LinkedIn feed:
   ```
   browser navigate → https://www.linkedin.com/feed/
   ```

2. Take snapshot, find the "Start a post" button, click it

3. In the post modal, find the textbox (usually the main content-editable area) and type your content

4. For **text-only posts**: Click "Post" button

5. For **posts with images**: Click the image/media icon in the post toolbar before posting, upload the file, then click Post

### Post Formatting Tips
- LinkedIn supports **bold** and *italic* via Unicode characters (not markdown)
- Use line breaks for readability
- Hashtags work: #SecurityResearch #AI
- Mentions: Type @ then select from dropdown
- Keep posts under 3000 characters (LinkedIn limit)
- First 2-3 lines are "above the fold" — make them count

## Checking Notifications

1. Navigate to `https://www.linkedin.com/notifications/`
2. Snapshot to read notification list
3. Click specific notifications to respond

## Checking Profile Analytics

1. Navigate to `https://www.linkedin.com/dashboard/` 
2. Or click "Show all analytics" from profile page
3. Shows: profile views, post impressions, search appearances

## Engagement (Like, Comment, Share)

### Liking a Post
- Snapshot the feed, find the Like button on target post, click it

### Commenting
- Click "Comment" button on post
- Type in the comment textbox
- Click "Post" (comment submit button)

### Sharing
- Click "Repost" button → select "Repost" or "Repost with your thoughts"

## Searching

Navigate to: `https://www.linkedin.com/search/results/all/?keywords=YOUR+SEARCH+TERMS`

## Profile Editing

Navigate to: `https://www.linkedin.com/in/YOUR-PROFILE-SLUG/edit/intro/`

## Common Gotchas

- LinkedIn aggressively detects automation — keep actions human-paced
- Post modal can take a moment to load — snapshot after clicking "Start a post"
- Image uploads need the file picker — use `browser upload` action
- LinkedIn may show CAPTCHAs — these need human intervention
- Session expires periodically — re-login if actions fail with redirect to login page
