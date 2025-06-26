
ELEVATION - Material Design

Dialog 24
Modal bottom sheet Modal side sheet 16
Navigation drawer 16
Floating action button (FAB - pressed) 12
Standard bottom sheet Standard side sheet 8
Bottom navigation bar 8
Bottom app bar 8
Menus and sub menus 8
Card (when picked up) 8
Contained button (pressed state) 8
Flating action button (FAB - resting elevation) Snackbar 6
Top app bar (scrolled state) 4
Top app bar (resting elevation) 0 or 4
Refresh indicator Search bar (scrolled state) 3
Contained button (resting elevation) 2
Search bar (resting elevation) 1
Card (resting elevation) 1
Switch 1
Text button 0
Standard side sheet 0

ELEVATION - Material layout

Screen size Margin Body Layout columns
Extra-small (phone)
0-599dp 16dp Scaling 4
Small (tablet)
600-904 32dp Scaling 8
905-1239 Scaling 840dp 12
Medium (laptop)
1240-1439 200dp Scaling 12
Large (desktop)
1440+ Scaling 1040 12

CSS FONTS

html {
font-family:
system-ui,
/* macOS 10.11-10.12 _/ -apple-system, /_ Windows 6+ _/ Segoe UI, /_ Android 4+ _/ Roboto, /_ Ubuntu 10.10+ _/ Ubuntu, /_ Gnome 3+ _/ Cantarell, /_ KDE Plasma 5+ _/ Noto Sans, /_ fallback _/ sans-serif, /_ macOS emoji _/ "Apple Color Emoji", /_ Windows emoji _/ "Segoe UI Emoji", /_ Windows emoji _/ "Segoe UI Symbol", /_ Linux emoji _/ "Noto Color Emoji"; } code, kbd, pre, samp { font-family: /_ macOS 10.10+ _/ Menlo, /_ Windows 6+ _/ Consolas, /_ Android 4+ _/ Roboto Mono, /_ Ubuntu 10.10+ _/ Ubuntu Monospace, /_ KDE Plasma 5+ _/ Noto Mono, /_ KDE Plasma 4+ _/ Oxygen Mono, /_ Linux/OpenOffice fallback _/ Liberation Mono, /_ fallback */ monospace;

Sample meta tags with preconnects

```
        <link rel="icon" type="image/png" href="/temporal-icon.png" />
        <meta name="theme-color" content="#317EFB"/>
        <meta property="title" content="Temporal.io: Build Invincible Apps" />
        <meta property="og:title" content="Temporal.io: Build Invincible Apps" />
        <meta name="description" content="Temporal is the open source runtime for running mission critical code that runs atop unreliable, distributed services at any scale." />
        <meta property="og:description" content="Temporal is the open source runtime for running mission critical code that runs atop unreliable, distributed services at any scale." />
        <meta property="og:image" content="<https://temporal.io/logo-font-straight-dark.svg>" />
        <meta property="og:url" content="<http://temporal.io>" />
        <meta property="twitter:title" content="Temporal.io: Build Invincible Apps" />
        <meta property="twitter:description" content="Temporal is the open source runtime for running mission critical code that runs atop unreliable, distributed services at any scale." />
        <meta property="twitter:image" content="<https://temporal.io/logo-font-straight-dark.svg>" />
        <meta property="twitter:card" content="summary_large_image" />
        <meta name="twitter:site" content="@temporaltech" />

        {/* resource hints */}
        <link rel="preconnect" href="<https://fonts.gstatic.com>" />
        <link rel="preconnect" href="<https://www.youtube.com>" />
        <link rel="preconnect" href="<https://yt3.ggpht.com>" />
        <link rel="preconnect" href="<https://static.doubleclick.net>" />
        <link rel="preconnect" href="<https://googleads.g.doubleclick.net>" />
        <link rel="preconnect" href="<https://i.ytimg.com>" />
        <link rel="preconnect" href="<https://s.ytimg.com>" />
        <link rel="preconnect" href="<https://www.google-analytics.com>" />

        <script
          async
          src="<https://www.googletagmanager.com/gtag/js?id=>[Tracking ID]"
        />

        <script
          dangerouslySetInnerHTML={{
            __html: `
                  window.dataLayer = window.dataLayer || [];
                  function gtag(){dataLayer.push(arguments);}
                  gtag('js', new Date());
                  gtag('config', '[Tracking ID]');
              `,
          }}
        />
```
