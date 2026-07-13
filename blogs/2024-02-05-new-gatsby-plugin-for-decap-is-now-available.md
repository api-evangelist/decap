---
title: "New Gatsby plugin for Decap is now available"
url: "https://decapcms.org/blog/new-gatsby-plugin-for-decap-is-now-available/"
date: "2024-02-05"
feed_url: "https://decapcms.org/blog/index.xml"
---
The deprecated gatsby-plugin-netlify-cms that corresponds to the old Netlify CMS package is now deprecated and replaced by gatsby-plugin-decap-cms . To migrate you Gatsby site from Netlify CMS 2 to Decap CMS 3: uninstall gatsby-plugin-netlify-cms and netlify-cms-app install gatsby-plugin-netlify-cms and decap-cms-app replace the import import CMS from "netlify-cms-app" with import CMS from "decap-cms-app" in gatsby config replace resolve: "gatsby-plugin-netlify-cms" with resolve: "gatsby-plugin-decap-cms" An example of a migration can be found in this PR on the Decap-Gatsby starter template .
