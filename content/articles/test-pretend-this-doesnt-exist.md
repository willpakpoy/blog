---
title: this is a test article
date: 2021-03-02
---

# this is a test article

**This is a `.md` file.**


**And this is the eleventy config.**
```
const pluginSass = require("eleventy-plugin-sass");

module.exports = function(eleventyConfig) {
    eleventyConfig.addPassthroughCopy("static");
    eleventyConfig.addWatchTarget("./styles/**/*");
    eleventyConfig.addPlugin(pluginSass, {sourcemaps: true});

    return {
      dir: {
        input: "content",
        includes: "../_includes",
        data: "../_data"
      }
    };
  
  };
```
