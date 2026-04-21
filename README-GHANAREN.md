# GhanaRent - Car Rental Website Documentation

## Overview
This is a complete car rental website for Ghana featuring an interactive fleet display and online booking system that sends booking requests directly to your email.

## Files Created

### 1. **index-rental.html** - Home Page
- Landing page with hero section
- Statistics/highlights section (50+ vehicles, 1000+ customers, etc.)
- Complete fleet showcase with 6 different vehicle types:
  - Toyota Corolla (Sedan)
  - Hyundai i10 (Economy)
  - Ford Ranger (Pickup)
  - Toyota Highlander (SUV)
  - Hyundai H350 (Van)
  - Mercedes-Benz C-Class (Premium)
- About section with company benefits
- Call-to-action section
- Professional navigation and footer

### 2. **booking-rental.html** - Booking Page
- Comprehensive booking form with:
  - Customer information section (name, email, phone, WhatsApp)
  - Booking details (vehicle type, dates, locations, duration)
  - Additional services options
  - Special requests field
- Form validation
- Professional layout with info boxes
- Redirects to thank-you page after submission

### 3. **contact-rental.html** - Contact Page
- Contact information cards (phone, email, WhatsApp)
- Branch locations across Ghana (Accra, Kumasi, Takoradi, Sekondi)
- Working hours for each branch
- Contact form for general inquiries
- Professional design matching the brand

### 4. **thank-you-rental.html** - Confirmation Page
- Confirmation message after booking
- Next steps information
- Animated success icon
- Quick links to navigate back or view more cars

## How to Set Up Email Functionality

### Step 1: Update Email Address
The website uses **FormSubmit.co** - a free email form service that requires NO backend setup!

In both **booking-rental.html** and **contact-rental.html**, find this line:
```
action="https://formsubmit.co/your-email@gmail.com"
```

Replace `your-email@gmail.com` with your actual email address.

### Step 2: First Submission
When someone submits a form:
1. FormSubmit will send a confirmation email to your inbox
2. Click the confirmation link in that email
3. All future form submissions will then be directed to your email automatically

### Step 3: Optional - Customize Email Settings
FormSubmit offers several optional features. To use them, add these hidden fields to the form:

```html
<!-- Redirect to thank-you page after 5 seconds -->
<input type="hidden" name="_next" value="thank-you-rental.html">

<!-- Add a subject line prefix -->
<input type="hidden" name="_subject" value="New GhanaRent Booking Request">

<!-- Disable CAPTCHA (FormSubmit adds it by default) -->
<input type="hidden" name="_captcha" value="false">

<!-- CC yourself on every email -->
<input type="hidden" name="_cc" value="your-backup-email@gmail.com">
```

## Customization Guide

### Update Company Information
Search and replace in all HTML files:

1. **Contact Numbers:**
   - Replace `+233 (0) XXX XXX XXX` with actual phone numbers

2. **Email Addresses:**
   - Replace `info@ghanaren.com` with your actual email
   - Replace `support@ghanaren.com` with support email

3. **Brand Name:**
   - Replace "GhanaRent" with your company name

### Modify Vehicle List
In **index-rental.html**, each vehicle is in a "car-card" div. To modify:

1. Change the icon: `<i class="fas fa-car"></i>` (see Font Awesome icons)
2. Update vehicle name and price
3. Modify specifications and features
4. Update the vehicle list in the booking form's select dropdown

### Update Branch Locations
In **contact-rental.html**, locate the branch cards and update:
- Branch name and region
- Address
- Phone number
- Working hours

## Features

✅ **Responsive Design** - Works on desktop, tablet, and mobile  
✅ **Professional Styling** - Modern gradient background, smooth animations  
✅ **Easy Booking** - Multi-step form with clear sections  
✅ **Email Integration** - Automatic email notifications (no backend needed)  
✅ **Fleet Management** - Display multiple vehicle types with pricing  
✅ **Contact Information** - Multiple contact methods (phone, email, WhatsApp)  
✅ **Branch Locations** - Show all rental locations in Ghana  
✅ **Animations** - Smooth hover effects and page animations  

## Navigation Structure

```
index-rental.html (Home)
├── Link to booking-rental.html (Book Now)
├── Link to index-rental.html#fleet (Our Fleet)
├── Link to contact-rental.html (Contact)
└── Link to index-rental.html#about (About)

booking-rental.html (Booking)
├── Form submission → thank-you-rental.html (Confirmation)
└── Links back to home

contact-rental.html (Contact)
├── Contact information
├── Branch locations
├── Contact form → thank-you-rental.html (Confirmation)
└── Links back to home
```

## Color Scheme

- **Primary Blue:** `#1e3a8a` - Headers, buttons, accents
- **Light Blue:** `#1e40af` - Gradients
- **Gold/Yellow:** `#ffc107` - Highlights, CTAs
- **White:** `#ffffff` - Backgrounds
- **Dark Gray:** `#333333` - Text
- **Light Gray:** `#f8f9fa` - Section backgrounds

## Font Icons Used
The website uses **Font Awesome 6.0.0** for icons. Common icons used:
- `fas fa-car` - Car icon
- `fas fa-map-marker-alt` - Location icon
- `fas fa-phone` - Phone icon
- `fas fa-envelope` - Email icon
- `fab fa-whatsapp` - WhatsApp icon
- `fas fa-check-circle` - Checkmark icon

## Testing the Website

1. **Open** index-rental.html in your web browser
2. **Navigate** through all pages using the menu
3. **Test the Booking Form:**
   - Fill out all fields
   - Click "Submit Booking Request"
   - You should receive an email confirmation to send to your address
4. **Verify Email:**
   - Check your inbox for the FormSubmit verification email
   - Click the confirmation link
   - Now all form submissions will work automatically

## Mobile Optimization

All pages are fully responsive:
- Menu collapses into hamburger on mobile
- Form input fields stack vertically
- Car cards display in single column on small screens
- Touch-friendly buttons and links
- Optimized font sizes for readability

## Browser Compatibility

Works on:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Tips

1. **Images:** Add vehicle images to `img/` folder and replace the icon placeholders
2. **Optimization:** Minify CSS and JavaScript for production
3. **Hosting:** Use a fast web hosting provider in Ghana or nearby
4. **SEO:** Update meta tags and keywords in HTML head sections

## Support & Issues

If forms aren't working:
1. Check that you've replaced the email address with YOUR actual email
2. Verify you clicked the confirmation link in the FormSubmit email
3. Check spam/filters folder for confirmation email
4. Test with a different email if needed

## Future Enhancements

Consider adding:
- Online payment integration (Ghana payment gateway)
- Admin dashboard to manage bookings
- Email notifications with booking details
- WhatsApp integration for alerts
- Insurance options in the booking form
- Customer reviews/testimonials section
- Blog section for travel tips
- Multi-language support (English/Twi)

---

**Created:** 2024  
**Based in:** Ghana  
**For:** Car Rental Business  

**Questions?** You can expand the website with more pages or integrate additional services as needed.
