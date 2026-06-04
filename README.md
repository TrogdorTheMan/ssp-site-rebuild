# Seattle Seafair Pirates — Site Rebuild

A ground-up static rebuild of [seafairpirates.org](https://seafairpirates.org), the official website of the Seattle Seafair Pirates.

## About the Project

The Seattle Seafair Pirates are a Seattle civic organization founded in 1949, best known for their annual theatrical "invasion" of the Seattle waterfront to open Seafair each summer. This project rebuilds their existing WordPress site as a clean, fast static site hosted on Azure Static Web Apps.

**Goals:**
- Replace the aging WordPress site with a lightweight, maintainable static HTML/CSS site
- Preserve and present the organization's rich history and photo archive
- Improve page performance and mobile experience
- Establish a modern foundation for future content updates

## About the Developer

This project is maintained by **TrogdorTheMan** — an IT professional and active member of the Seattle Seafair Pirates. Beyond delivering a better website for the organization, this project is also a hands-on exploration of how AI tools can be practically applied in real-world scenarios and web development work. Building alongside AI (specifically Claude Code) is as much a part of the goal as the site itself.

## Tech Stack

- Plain HTML5 & CSS3 — no frameworks, no build step
- Fonts via Google Fonts (Playfair Display, Crimson Pro, Space Mono)
- Leaflet.js for the interactive 2026 Destinations map
- Images served from the existing seafairpirates.org CDN until go-live
- Deployment: Azure Static Web Apps (free tier)

## Deployment

Deployment is via the GitHub Actions workflow at `.github/workflows/azure-static-web-apps.yml`. The workflow is currently set to manual trigger (`workflow_dispatch`) only — it will be re-enabled for automatic deployment on push once the Azure Static Web App resource and API token are in place.

**To deploy:**
1. Create an Azure Static Web App resource (free tier)
2. Add the deployment token as `AZURE_STATIC_WEB_APPS_API_TOKEN` in GitHub repo secrets
3. Re-enable the `push` trigger in the workflow file

## Pages

### Our History
| Page | File |
|---|---|
| Home | `index.html` |
| Seattle Seafair Pirates | `seattle-seafair-pirates.html` |
| The Washington State Press Club | `washington-state-press-club.html` |
| The Ale & Quail Society | `ale-and-quail-society.html` |
| The Moby Duck | `the-moby-duck.html` |
| Captain Kidd — Past to Present | `captain-kidd.html` |
| History in Pictures | `our-history-in-pictures.html` |

### Destinations
| Page | File |
|---|---|
| 2026 Destinations | `2026-destinations.html` |

### Seafair
| Page | File |
|---|---|
| The Birth of Seafair | `the-birth-of-seafair.html` |
| Signature Seafair Events | `signature-seafair-events.html` |
| Seafair Volunteer Groups | `seafair-volunteer-groups.html` |
| More Seafair Traditions | `more-seafair-traditions.html` |
| The Legend of Seafair (1953) | `the-legend-of-seafair-1953.html` |
| The Legend of Seafair (1954) | `the-legend-of-seafair-1954.html` |

### Gallery
| Page | File |
|---|---|
| Gallery of Rogues | `gallery-of-rogues.html` |
| Then & Now | `then-and-now.html` |
| Videos | `videos.html` |

### Other
| Page | File |
|---|---|
| Sponsors | `sponsors.html` |
| 404 | `404.html` |
