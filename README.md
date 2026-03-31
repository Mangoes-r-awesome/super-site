# Super — Website

Deploy to Vercel:
1. Push this folder to a GitHub repo
2. Import to Vercel at vercel.com/new
3. Add your custom domain in Vercel settings

Or use CLI:
```
cd super-site
npx vercel --prod
```

## Structure
- public/index.html — Single-page app (all pages)
- public/img/ — Property + team photos
- vercel.json — Vercel config

## To customize
- Edit index.html in any text editor
- Replace YouTube placeholder URL in Work With Us video section
- Hostaway widget is already wired to book.superhostly.com.au
- Add more property photos to /img/ and update the card references

## Hostaway Calendar Widget (per-listing)
Add to individual property pages:
```html
<div id="hostaway-calendar-widget"></div>
<script src="https://d2q3n06xhbi0am.cloudfront.net/calendar.js"></script>
<script>
  window.hostawayCalendarWidget({
    baseUrl: 'https://book.superhostly.com.au/',
    listingId: YOUR_LISTING_ID,
    numberOfMonths: 2,
    color: { mainColor: '#E8593C' },
  })
</script>
```
