# SnapStudio

SnapStudio is a front-end prototype for a photography platform. Clients can browse photographers' portfolios, book sessions and sign up for photography events. Photographers can log in to post and manage their work.

It's built with HTML, CSS and [Bootstrap 5](https://getbootstrap.com/), and the pages are responsive.

> This is a static prototype. Forms, search, filters and the login don't send or save any data.

## Pages

| Page | File | Description |
|------|------|-------------|
| Home / About | `index.html` | Hero banner, plus an overview of the showcase, posting and events features |
| Portfolio Showcase | `vendor_gallery.html` | Grid of photographers with a bio and availability on hover |
| Book a Session | `item_details.html` | Choose a photographer or workshop and a date and time, then add the booking to the cart |
| Checkout | `checkout.html` | Customer details and order summary |
| Events | `event.html` | Upcoming photography workshops |
| Post Your Work (Login) | `login.html` | Photographer sign-in |
| Vendor Management | `vendor_management.html` | Photographer dashboard for uploading, editing and deleting posts |

Every page shares the same navigation bar (with category, location and price filters and a search bar) and the same footer (with an embedded Google Map).

## Project structure

```
.
├── index.html
├── vendor_gallery.html
├── item_details.html
├── checkout.html
├── event.html
├── login.html
├── vendor_management.html
├── css/
│   └── style.css            # Custom styles
├── img/                     # Site images
└── bootstrap-5.3.7-dist/    # Local copy of Bootstrap
```

## Running locally

You don't need to build or install anything. Clone the repo and open `index.html` in a browser:

```bash
git clone https://github.com/Kuwakou/snap-studio.git
cd snap-studio
open index.html
```

You can also serve the folder with a local server, such as the VS Code **Live Server** extension or this command:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

An internet connection is required, because the pages load Bootstrap from the jsDelivr CDN and the map from Google Maps.

## Built with

- HTML5
- CSS3
- Bootstrap 5.3
