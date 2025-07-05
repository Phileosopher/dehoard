
Ideas of things you can include based on my own site.

```
  <link rel="icon" type="image/png" href="/favicon.png" />
  <link rel="webmention" href="<https://webmention.io/www.swyx.io/webmention>" />
  <link rel="pingback" href="<https://webmention.io/www.swyx.io/xmlrpc>" />
  <meta name="theme-color" content="#818CF8">
  <title>{frontmatter.title} ∊ swyx.io</title>
  <link rel="canonical" href={canonical} />
  <meta property="og:url" content={swyxioURL} />
  <meta property="og:type" content="article" />
  <meta property="og:title" content={seoTitle} />
  <meta name="Description" content={seoDescription} />
  <meta property="og:description" content={seoDescription} />
  {#if frontmatter.cover_image}
    <meta property="og:image" content={coverImage} />
  {/if}
  <meta
    name="twitter:card"
    content={frontmatter.cover_image ? 'summary_large_image' : 'summary'} />
  <meta name="twitter:domain" content="swyx.io" />
  <meta name="twitter:creator" content="@swyx" />
  <meta name="twitter:title" content={seoTitle} />
  <meta name="twitter:description" content={seoDescription} />
  <meta
    name="twitter:image"
    content={frontmatter.cover_image ? frontmatter.cover_image : '<https://www.swyx.io/swyx-ski.jpeg>'} />
  <meta name="twitter:label1" value="Last updated" content="Last updated" />
  <meta name="twitter:data1" value={metaDate} content={metaDate} />
  <meta name="twitter:label2" content="Read Time" />
  <meta name="twitter:data2" content={readTime} />
```
