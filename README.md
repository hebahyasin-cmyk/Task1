# Reverifi Home Webpage 

## Project Overview
Reverifi is a real estate platform that allows users to search and connect with trusted real estate professionals, view featured listings, and explore events. This project includes a responsive HTML structure for both mobile and desktop views, along with CSS styling and assets.

---

## Project Structure
```
Task1/
│
├─ index.html # Main HTML page
├─ style.css # Main stylesheet
├─ assets/ # All images and icons
│   ├─ header/
│   │   └─ primary-logo.svg
│   ├─ search-listing/
│   │   ├─ search-icon.svg
│   │   └─ search-image.svg
│   ├─ featured-listing/
│   │   ├─ featured-image-1.png
│   │   ├─ featured-image-2.svg
│   │   └─ featured-image-3.svg
│   └─ ... (other icons/images)
└─ README.md # Developer documentation
```
---

## HTML Structure
```
html (lang="en")
├── head
│   ├── meta (charset="UTF-8")
│   ├── title ("Home Page")
│   ├── meta (name="description")
│   ├── meta (name="author" content="Hebah Yasin")
│   ├── meta (name="keywords")
│   ├── meta (name="viewport")
│   ├── link (rel="stylesheet" href="style.css")
│   └── link (href="Google Fonts - Montserrat")
│
├── body
│   ├── header.mobile
│   │   ├── button.menu-toggle
│   │   │   ├── span
│   │   │   ├── span
│   │   │   └── span
│   │   └── img (src="assets/header/primary-logo.svg")
│   │
│   ├── header.desktop
│   │   └── div.desktop-header-container
│   │       ├── div.left-container
│   │       │   ├── img (src="assets/header/primary-logo.svg")
│   │       │   └── nav.nav
│   │       │       ├── a (href="#" - "How we Work")
│   │       │       ├── a (href="#" - "Find an Agent")
│   │       │       └── a (href="#" - "Knowledge Center")
│   │       └── div.right-container
│   │           ├── button.btn.sign ("Sign In")
│   │           └── button.btn.join ("Join Now")
│   │
│   ├── main
│   │   ├── section.search-listing
│   │   │   ├── div.search-listing-text
│   │   │   │   ├── h1 ("Search our listings...")
│   │   │   │   └── div.search-box
│   │   │   │       ├── input (type="search")
│   │   │   │       └── button.search-btn (type="submit")
│   │   │   │           └── img (src="search-icon.svg")
│   │   │   └── img.search-listing-img (src="search-image.svg")
│   │   │
│   │   ├── section.featured-listing
│   │   │   ├── h2 ("Our Featured Listing")
│   │   │   ├── div.carousel
│   │   │   │   └── div.featured-grid
│   │   │   │       ├── div.featured-listing-card (x3)
│   │   │   │       │   ├── div.card-img
│   │   │   │       │   │   ├── img (src="featured-image-*.svg/png")
│   │   │   │       │   │   ├── div.flag-wrapper
│   │   │   │       │   │   │   └── div.card-img-flag.new/rent
│   │   │   │       │   │   └── div.card-img-person
│   │   │   │       │   └── div.card-text
│   │   │   │       │       ├── div.card-text-content
│   │   │   │       │       │   ├── div.card-text-left
│   │   │   │       │       │   │   ├── span.listing-title
│   │   │   │       │       │   │   ├── span.listing-location
│   │   │   │       │       │   │   └── div.listing-services
│   │   │   │       │       │   │       ├── span.service-bed
│   │   │   │       │       │   │       ├── span.service-wifi
│   │   │   │       │       │   │       ├── span.service-bath
│   │   │   │       │       │   │       ├── span.service-condition
│   │   │   │       │       │   │       └── span.service-furniture
│   │   │   │       │       │   └── div.card-text-right
│   │   │   │       │       │       └── span.listing-distance
│   │   │   │       │       ├── hr
│   │   │   │       │       └── div.card-text-footer
│   │   │   │       │           ├── span.listing-price
│   │   │   │       │           └── div.listing-share
│   │   │   │       │               ├── button.icon-btn.like
│   │   │   │       │               │   └── svg (heart icon)
│   │   │   │       │               └── button.icon-btn.share
│   │   │   │       │                   └── svg (share icon)
│   │   │   └── div.circles
│   │   │       ├── div.circle.active
│   │   │       └── div.circle (x6)
│   │   │
│   │   ├── section.events
│   │   │   ├── h2 ("Events")
│   │   │   ├── nav
│   │   │   │   ├── a.event-status (href="#" - "all")
│   │   │   │   ├── a.event-status (href="#" - "upcoming")
│   │   │   │   └── a.event-status (href="#" - "past")
│   │   │   └── div.carousel
│   │   │       ├── button.carousel-btn.prev
│   │   │       │   └── svg (left arrow)
│   │   │       ├── button.carousel-btn.next
│   │   │       │   └── svg (right arrow)
│   │   │       └── div.events-grid
│   │   │           └── div.event-card (x4)
│   │   │               ├── div.flag-wrapper
│   │   │               │   └── div.card-img-flag.personal/webiner
│   │   │               ├── div.card-img-date
│   │   │               ├── div.card-content
│   │   │               │   └── div.event-info
│   │   │               │       ├── span.event-title
│   │   │               │       └── div.event-time
│   │   │               │           └── span
│   │   │               └── div.card-footer
│   │   │                   ├── div.event-action
│   │   │                   │   ├── button.icon-btn.add
│   │   │                   │   │   └── svg (plus icon)
│   │   │                   │   └── button.icon-btn.share
│   │   │                   │       └── svg (share icon)
│   │   │                   └── span.people
│   │   │
│   │   ├── section.search-network
│   │   │   ├── div.search-network-text
│   │   │   │   ├── h2 ("reverifi")
│   │   │   │   ├── p
│   │   │   │   └── button ("See More")
│   │   │   └── div.search-network-teams
│   │   │       ├── span ("Attorney")
│   │   │       ├── span ("Photographer")
│   │   │       ├── span ("Agent")
│   │   │       ├── span ("Cleaning Services")
│   │   │       ├── span ("Home Inspectors")
│   │   │       └── span ("Insurance Provider")
│   │   │
│   │   ├── section.explore
│   │   │   ├── h2 ("Explore our Listings")
│   │   │   ├── div.card-container
│   │   │   │   └── div.card (x7)
│   │   │   │       ├── img (src="location.svg")
│   │   │   │       ├── div.img-overlay
│   │   │   │       └── div.explore-text
│   │   │   │           ├── span (location name)
│   │   │   │           └── span (listing count)
│   │   │   └── div.circles
│   │   │       ├── div.circle.active
│   │   │       └── div.circle (x6)
│   │   │
│   │   └── section.claim-address
│   │       └── div.map
│   │           └── div.map-content
│   │               ├── svg.pin-icon
│   │               └── div.text-content
│   │                   ├── h2 ("Claim your Address")
│   │                   └── div.search-box
│   │                       ├── input (type="search")
│   │                       ├── button.search-btn.mobile
│   │                       │   └── img
│   │                       └── button.search-btn.desktop
│   │                           └── svg (arrow icon)
│   │
│   └── footer
│       ├── div.join-us
│       │   └── div.join-us-text-content
│       │       ├── h3
│       │       └── button ("Join us")
│       ├── div.contact
│       │   └── div.contact-container
│       │       ├── div.social-media
│       │       │   ├── span (x4 - social media icons)
│       │       ├── div.media
│       │       │   ├── div.traditional-contact
│       │       │   │   ├── img (logo)
│       │       │   │   ├── span (phone 1)
│       │       │   │   ├── span (email)
│       │       │   │   └── span (phone 2)
│       │       │   ├── div.links (x3)
│       │       │   │   ├── h3 (section title)
│       │       │   │   └── span (link items)
│       │       │   └── div.links (newsletter)
│       │       │       ├── h3
│       │       │       ├── div.subscribe-bar.mobile
│       │       │       │   ├── label
│       │       │       │   └── button
│       │       │       └── div.subscribe-bar.desktop
│       │       │           ├── span
│       │       │           └── button
│       └── div.license
```
