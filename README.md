# SRGP Realty Website

A property listings website for **SRGP Realty**, a real estate advisor based in Kompally, Hyderabad. Visitors can browse apartments, villas, open plots and farm land, open a page for each project, and send an enquiry that reaches SRGP Realty straight away.

**Live site:** _add the Netlify link here, for example https://srgprealty.netlify.app_

## What the website does

- **Homepage** with a photo slideshow, property categories (Apartments, Villas, Open Plots, Farm Land), search, filters (type, locality, budget, status) and sorting
- **A page for every project** with:
  - key details: builder, RERA number, land area, units, possession and facing
  - a photo gallery that opens full screen, including master plans and floor plans
  - project videos
  - a price table for every flat or plot size
  - a home loan EMI calculator
  - amenities, specifications and travel times to nearby places
  - an enquiry form
- **Enquiry forms** that send each lead to a Google Sheet and an email alert
- **Shortlist** so visitors can save the projects they like
- Works on phones, tablets and computers

## Current projects

| Project | Type | Location |
|---|---|---|
| North Crest | Apartments | Kompally |
| Emerald Heights | Apartments | Kompally |
| Vistara's Delight Heights | Apartments | Kompally |
| Dhatri County-II | Villa plots | Railapur, Kompally |
| Nature Orchid II | Open plots | Bhongir |

## How it is built

| Part | Technology |
|---|---|
| Website | HTML, CSS and JavaScript in a single `index.html` file, with no frameworks |
| Photos and videos | `images/` folder |
| Enquiries | Google Apps Script that adds each enquiry to a Google Sheet and sends an email |
| Code storage | GitHub (this repository) |
| Hosting | Netlify, which republishes the site automatically when this repository changes |

All project information is kept in one list, `LISTINGS`, inside `index.html`. Each project's card and page are built automatically from that list, so adding a project or changing a price means editing that one place.

## How the website was made

I planned the website and collected the content: builder brochures, floor plans, posters, project videos and contact details. I built it with **Claude**, an AI assistant made by Anthropic. Claude:

- wrote the website code
- read the project details from the brochures, including flat sizes from the floor plans
- prepared the photos and videos
- tested the site on desktop and phone screens

I checked the information, decided what goes on the site, and set up GitHub, Netlify and the Google Sheet.

## Project structure

```
index.html      the whole website: layout, styles, project data and code
images/         project photos, floor plans, videos and the SRGP logo
README.md       this file
```

## Updating the website

1. Edit `index.html`, or add new photos and videos inside `images/`.
2. Upload the changed files to this repository and commit.
3. Netlify updates the live site within about a minute.

## Contact

**SRGP Realty**, Real Estate Advisor
Gundlapochampally, Kompally, Telangana 500100
Phone: +91 90592 58889 · +91 85000 23333
Email: realtysrgp@gmail.com

---

_Project images are artist's impressions from the builders' brochures. Prices, sizes and availability are subject to change; please confirm with SRGP Realty before booking._
