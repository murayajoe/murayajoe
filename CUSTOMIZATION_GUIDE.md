# 🎨 GitHub Profile Customization Guide

This guide will help you personalize and extend your GitHub profile beyond the default setup.

---

## 🌈 Changing Color Schemes

### Current Theme
Your profile uses the **Tokyo Night** theme with custom colors:
- Background: `#0D1117`
- Primary: `#F85D7F` (pink/red)
- Secondary: `#F8D866` (yellow/gold)

### Available Stat Card Themes
Replace `theme=tokyonight` with any of these:

| Theme Name | Style |
|------------|-------|
| `default` | GitHub's default |
| `dark` | Dark theme |
| `radical` | Radical purple |
| `merko` | Green matrix style |
| `gruvbox` | Retro gruvbox |
| `tokyonight` | Current theme |
| `onedark` | Atom One Dark |
| `cobalt` | Cobalt blue |
| `synthwave` | Synthwave purple |
| `highcontrast` | High contrast |
| `dracula` | Dracula theme |
| `prussian` | Prussian blue |
| `monokai` | Monokai |
| `vue` | Vue green |
| `vue-dark` | Vue dark |
| `shades-of-purple` | Purple theme |
| `nightowl` | Night Owl |
| `buefy` | Buefy teal |
| `blue-green` | Blue-green gradient |
| `algolia` | Algolia blue |
| `great-gatsby` | Gatsby purple |
| `darcula` | JetBrains Darcula |
| `bear` | Bear brown |
| `solarized-dark` | Solarized Dark |
| `solarized-light` | Solarized Light |
| `chartreuse-dark` | Chartreuse theme |
| `nord` | Nord theme |
| `gotham` | Gotham theme |
| `material-palenight` | Material Palenight |
| `graywhite` | Gray & White |
| `vision-friendly-dark` | Vision-friendly |
| `ayu-mirage` | Ayu Mirage |
| `midnight-purple` | Midnight Purple |
| `calm` | Calm theme |
| `flag-india` | India flag colors |
| `omni` | Omni theme |
| `react` | React blue |
| `jolly` | Jolly theme |
| `maroongold` | Maroon & Gold |
| `yeblu` | Yellow & Blue |
| `blueberry` | Blueberry theme |
| `slateorange` | Slate & Orange |
| `kacho_ga` | Kacho ga theme |

### How to Change Theme
Find all instances of `theme=tokyonight` in README.md and replace with your preferred theme.

**Example:**
```markdown
<!-- Before -->
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=murayajoe&theme=tokyonight)

<!-- After -->
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=murayajoe&theme=dracula)
```

### Custom Colors
You can also use custom colors:

```markdown
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=murayajoe&bg_color=0D1117&title_color=F85D7F&icon_color=F8D866&text_color=FFFFFF&border_color=F85D7F)
```

**Parameters:**
- `bg_color` - Background color (hex without #)
- `title_color` - Title text color
- `icon_color` - Icon color
- `text_color` - Body text color
- `border_color` - Border color
- `hide_border=true` - Remove border entirely

---

## ➕ Adding/Removing Sections

### Remove a Section
Simply delete the entire section from README.md, including the header and content.

**Example: Remove Gaming Section**
Delete these lines:
```markdown
## 🎮 Gaming & Content Creation
... (entire table and content)
---
```

### Add a New Section

#### Example: Add a Certifications Section
```markdown
## 🏆 Certifications & Achievements

- 🎓 **Odoo Certified Developer** - Odoo (2024)
- ☁️ **AWS Certified Solutions Architect** - Amazon Web Services
- 🐍 **Python Professional Certificate** - Python Institute
- 📊 **PostgreSQL Database Administration** - PostgreSQL Certification

---
```

#### Example: Add a Skills Progress Section
```markdown
## 📈 Skills Progress

```json
{
  "Odoo Development": "████████████████████ 95%",
  "Python": "█████████████████░░░ 90%",
  "JavaScript": "███████████████░░░░░ 85%",
  "DevOps": "████████████░░░░░░░░ 75%",
  "UI/UX Design": "██████████░░░░░░░░░░ 65%"
}
```
```

---

## 🔗 Updating Social Links

### Add New Social Platform
1. Go to [Shields.io](https://shields.io/)
2. Find your platform badge or create custom one
3. Add to the "Connect With Me" section

**Example: Add Discord**
```markdown
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/your-server)
```

### Remove Social Platform
Simply delete the badge line from the "Connect With Me" section.

### Update Existing Links
Find the badge and update the URL in parentheses:
```markdown
[![LinkedIn](badge-url)](YOUR-NEW-LINK-HERE)
```

---

## 🏷️ Adding Tech Stack Badges

### Find Badges
Visit [Shields.io](https://shields.io/) or [Badges 4 README](https://github.com/alexandresanlim/Badges4-README.md-Profile)

### Badge Template
```markdown
![TECH_NAME](https://img.shields.io/badge/DISPLAY_TEXT-HEX_COLOR?style=for-the-badge&logo=LOGO_NAME&logoColor=COLOR)
```

### Popular Tech Badges

#### Frontend
```markdown
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![Svelte](https://img.shields.io/badge/Svelte-FF3E00?style=for-the-badge&logo=svelte&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
```

#### Backend
```markdown
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
```

#### Cloud & DevOps
```markdown
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
```

#### Databases
```markdown
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white)
![Cassandra](https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache-cassandra&logoColor=white)
![ElasticSearch](https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white)
```

---

## ⏰ Modifying GitHub Action Schedules

### Cron Syntax
```
* * * * *
│ │ │ │ │
│ │ │ │ └─── Day of week (0-7, Sunday = 0 or 7)
│ │ │ └───── Month (1-12)
│ │ └─────── Day of month (1-31)
│ └───────── Hour (0-23)
└─────────── Minute (0-59)
```

### Common Schedules

| Description | Cron Expression |
|-------------|-----------------|
| Every 30 minutes | `*/30 * * * *` |
| Every hour | `0 * * * *` |
| Every 2 hours | `0 */2 * * *` |
| Every 6 hours | `0 */6 * * *` |
| Every 12 hours | `0 */12 * * *` |
| Daily at midnight | `0 0 * * *` |
| Daily at 9 AM | `0 9 * * *` |
| Twice daily (9 AM & 9 PM) | `0 9,21 * * *` |
| Every Monday at 9 AM | `0 9 * * 1` |
| First day of month | `0 0 1 * *` |

### Update Workflow Schedule
Edit the workflow file and change the cron value:

**Example: Change YouTube updates to every 2 hours**
```yaml
# In .github/workflows/blog-post-workflow.yml
on:
  schedule:
    - cron: '0 */2 * * *'  # Changed from '0 * * * *'
```

---

## 📊 Advanced Stat Card Customization

### Hide Specific Stats
```markdown
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=murayajoe&hide=issues,prs&theme=tokyonight)
```

**Options to hide:**
- `issues` - Hide issues count
- `prs` - Hide pull requests
- `contribs` - Hide contributions
- `commits` - Hide commits

### Show Private Contributions
```markdown
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=murayajoe&count_private=true&theme=tokyonight)
```

### Show All Languages (No Limit)
```markdown
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=murayajoe&layout=compact&langs_count=10&theme=tokyonight)
```

### Exclude Languages
```markdown
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=murayajoe&hide=html,css&theme=tokyonight)
```

### Compact Language Layout
```markdown
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=murayajoe&layout=compact&theme=tokyonight)
```

---

## 🎵 Optional: Add Spotify Integration

### Show Now Playing
1. Set up [Spotify GitHub Profile](https://github.com/kittinan/spotify-github-profile)
2. Follow the setup instructions to get your token
3. Add to README:

```markdown
## 🎵 Currently Vibing To

[![Spotify](https://spotify-github-profile.vercel.app/api/view?uid=YOUR_SPOTIFY_ID&cover_image=true&theme=novatorem&show_offline=false&background_color=0d1117&interchange=true&bar_color=f85d7f&bar_color_cover=true)](https://spotify-github-profile.vercel.app/api/view?uid=YOUR_SPOTIFY_ID&redirect=true)
```

---

## ⏱️ Optional: Add WakaTime Stats

### Show Coding Time Stats
1. Sign up at [WakaTime](https://wakatime.com/)
2. Install WakaTime plugin in your IDE
3. Get your API key from WakaTime dashboard
4. Add to GitHub secrets: `WAKATIME_API_KEY`
5. Create `.github/workflows/waka-readme.yml`:

```yaml
name: Waka Readme

on:
  schedule:
    - cron: '0 0 * * *'
  workflow_dispatch:

jobs:
  update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
      - uses: anmol098/waka-readme-stats@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          SHOW_PROJECTS: "True"
          SHOW_LANGUAGE: "True"
          SHOW_TIMEZONE: "True"
          SHOW_EDITORS: "True"
```

6. Add to README:
```markdown
## ⏱️ Coding Stats

<!--START_SECTION:waka-->
<!--END_SECTION:waka-->
```

---

## 🌟 Optional: Add GitHub Profile 3D Contrib

Create a 3D visualization of your contributions:

```yaml
# .github/workflows/profile-3d.yml
name: GitHub-Profile-3D-Contrib

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    name: generate-github-profile-3d-contrib
    steps:
      - uses: actions/checkout@v3
      - uses: yoshi389111/github-profile-3d-contrib@0.7.1
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          USERNAME: murayajoe
      - name: Commit & Push
        run: |
          git config user.name github-actions
          git config user.email github-actions@github.com
          git add -A .
          git commit -m "generated"
          git push
```

Add to README:
```markdown
## 🎨 3D Contribution Graph

![3D Contribution Graph](./profile-3d-contrib/profile-night-rainbow.svg)
```

---

## 🎯 Add Profile Page Views Analytics

Add detailed analytics using [Hits](https://hits.seeyoufarm.com/):

```markdown
![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fmurayajoe&count_bg=%23F85D7F&title_bg=%230D1117&icon=github.svg&icon_color=%23F8D866&title=Profile+Views&edge_flat=false)
```

---

## 🔄 Dynamic Quote Sources

Change the quote style in the README:

### Programming Quotes
```markdown
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight)
```

### Inspirational Quotes
```markdown
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight&quote=Inspirational)
```

### Random Quote Types
- `type=horizontal` - Horizontal layout
- `type=vertical` - Vertical layout
- `quote=Programming` - Programming quotes (default)
- `quote=Inspirational` - Motivational quotes

---

## 🎨 Capsule Render Customization

### Header Types
Change `type=waving` to:
- `wave` - Wave animation
- `waving` - Waving effect (current)
- `cylinder` - 3D cylinder
- `rounded` - Rounded corners
- `shark` - Shark fin shape
- `slice` - Slice design
- `rect` - Rectangle
- `soft` - Soft edges
- `transparent` - Transparent background

### Custom Colors
```markdown
![Header](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12&height=300&section=header&text=Your%20Name&fontSize=90)
```

**Gradient Numbers (customColorList):**
- `0-29` - Different gradient combinations
- Try different numbers to find your favorite

---

## 🚀 Pro Tips

### 1. Keep It Fast
- Don't add too many large GIFs
- Optimize image sizes
- Limit external API calls

### 2. Mobile Responsive
- Use `<div align="center">` for centering
- Keep table widths reasonable
- Test on mobile GitHub app

### 3. Accessibility
- Add alt text to images
- Use clear, readable fonts
- Ensure good color contrast

### 4. Regular Updates
- Update goals quarterly
- Refresh project pins
- Keep social links current
- Update tech stack as you learn

### 5. Performance
- Use CDN-hosted images
- Leverage Vercel/GitHub caching
- Don't query APIs too frequently

---

## 📚 Additional Resources

### Badge Generators
- [Shields.io](https://shields.io/) - Custom badges
- [Simple Icons](https://simpleicons.org/) - Brand icons
- [Badges 4 README](https://github.com/alexandresanlim/Badges4-README.md-Profile) - Pre-made badges

### Stat Generators
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [GitHub Readme Streak Stats](https://github.com/DenverCoder1/github-readme-streak-stats)
- [GitHub Profile Trophy](https://github.com/ryo-ma/github-profile-trophy)
- [Activity Graph](https://github.com/Ashutosh00710/github-readme-activity-graph)

### Animations
- [Typing SVG](https://github.com/DenverCoder1/readme-typing-svg)
- [Capsule Render](https://github.com/kyechan99/capsule-render)
- [Snake Game](https://github.com/Platane/snk)

### Inspiration
- [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [GitHub Profile README Generator](https://rahuldkjain.github.io/gh-profile-readme-generator/)

---

## 💡 Need More Help?

- Check the official documentation links above
- Explore other GitHub profiles for inspiration
- Join developer communities for profile feedback
- Experiment with different layouts and themes

**Remember**: Your profile is your digital portfolio - keep it updated and reflective of your current skills and projects! 🌟
