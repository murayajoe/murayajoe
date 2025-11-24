# How to Get Your YouTube Channel ID

## Quick Method (Browser)

1. Go to your channel: https://www.youtube.com/@senpaicodeske
2. Right-click anywhere on the page
3. Select **"View Page Source"** (or press `Ctrl+U`)
4. Press `Ctrl+F` to open search
5. Search for: `"channelId"`
6. You'll see something like: `"channelId":"UCxxxxxxxxxxxxxxxxxxxxx"`
7. Copy the ID (the part between quotes after `channelId":`)

## Alternative Method (YouTube Studio)

1. Go to [YouTube Studio](https://studio.youtube.com)
2. Click **Settings** (gear icon)
3. Click **Channel** → **Advanced settings**
4. Your Channel ID is shown at the bottom

## Alternative Method (Channel About Page)

1. Go to your channel: https://www.youtube.com/@senpaicodeske
2. Click the **About** tab
3. Click **Share channel** → **Copy channel ID**

---

## After Getting Your Channel ID

Replace the channel ID in the workflow file:

**File**: `.github/workflows/blog-post-workflow.yml`
**Line**: 21

Replace `UCZQFSqMyGP0mW3-9pZYJnqw` with your actual channel ID.

Or you can use this command:

```bash
cd "C:\Users\joemu\OneDrive - Anqad Systems Ltd\Desktop\gut muraya\murayajoe"

# Replace YOUR_CHANNEL_ID with the actual ID you found
sed -i 's/UCZQFSqMyGP0mW3-9pZYJnqw/YOUR_ACTUAL_CHANNEL_ID/' .github/workflows/blog-post-workflow.yml
```

---

## Test Your RSS Feed

Once you have your channel ID, test if it works:

Open this URL in your browser (replace with your ID):
```
https://www.youtube.com/feeds/videos.xml?channel_id=YOUR_CHANNEL_ID
```

You should see an XML feed with your latest videos.
