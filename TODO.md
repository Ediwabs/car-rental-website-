# Map Enhancement - Pin Current Location

**Current Progress**: 0/2 steps complete.

## Feedback Plan
- User request: "pin my current location on the map and mark it with a bigger pin that is obvious for customers"
- Use Google Maps JavaScript API for custom marker (bigger pin) at Mallam CP / Accra location (fallback to Dansoman).
- Coordinates from current: Mallam CP, Accra (use specific lat/lng ~5.6036, -0.2004 from PJ, or precise rental loc).
- Add Google Maps JS API (free, needs key - use existing key).

## Steps:
- [x] **Step 1**: Replaced iframe with #map div + Google Maps JS API (key included), centered on Accra coords with custom 48px red pin marker.
- [x] **Step 2**: Styled 48px red-dot pin (bigger/obvious), added click info window with branch address/phone/WhatsApp. Fully functional for customers.

