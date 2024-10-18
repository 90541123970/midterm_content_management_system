# midterm_content_management_system
 ## Apps Used
1. **Cookie Consent Banner**  
   - Description: This app was used to display the GDPR cookie consent banner on the store.  
   - URL: [Cookie Consent Banner](https://apps.shopify.com/cookie-consent-banner)
   <div id="gdpr-cookie-banner" style="position: fixed; bottom: 0; width: 100%; background-color: #333; color: white; text-align: center; padding: 15px; display: none;">
  <p style="margin: 0;">
    We use cookies to improve your experience on our site. By using our site, you consent to cookies. 
    <a href="/pages/privacy-policy" style="color: #fff; text-decoration: underline;">Learn more</a>
  </p>
  <button id="gdpr-accept" style="background-color: #4CAF50; border: none; color: white; padding: 10px 20px; margin-left: 10px; cursor: pointer;">Accept</button>
</div>

<script>
  document.addEventListener('DOMContentLoaded', function () {
    var gdprBanner = document.getElementById('gdpr-cookie-banner');
    var gdprAcceptBtn = document.getElementById('gdpr-accept');
    
    // Check if consent is already given
    if (!localStorage.getItem('gdprConsent')) {
      gdprBanner.style.display = 'block';
    }

    // When 'Accept' is clicked
    gdprAcceptBtn.addEventListener('click', function () {
      localStorage.setItem('gdprConsent', true);
      gdprBanner.style.display = 'none';
    });
  });
</script>
I Add map in contact us page(<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2889.555960655533!2d-79.64182212472794!3d43.59496455619677!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x882b47005b512105%3A0xcb124393cc3adfd5!2sAlgonquin%20College%20at%20CDI%20Campus!5e0!3m2!1sen!2sca!4v1729293444216!5m2!1sen!2sca" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>)

  aslo add  [product reviews']

## Customizations
1. **Featured Product Layout Change:** The product title was moved below the image on the homepage featured product section.
2. **GDPR Banner:** A dismissible GDPR consent banner was added to the site.
3. **Shopping Cart Layout Change:** The quantity column was moved before the price column, and the 'Update Cart' button was moved before the 'Continue Shopping' button.
4. **Animation:** Slide-in-from-left animation was applied to the footer sections for dynamic page interactions.

## Instructions for Reviewers
- To view the collections, click on the 'one collection ' so you can view all collection from the selected one in the main menu.
- You can navigate to the 'Contact Us,FAQS,About us,Collections, privacy as well' page from the footer or main menu to see the contact form.
- Social media sharing options are available on individual product pages also on the footer of the page.


## Theme Customization Details
- **Theme Style**: Modern
- **GDPR Banner**: firstly i install it from the app store then i did the code in theme.liquid.
- **Header Elements**:
  - Logo
  - Main menu with links to three collections and a contact form.
- **Homepage Includes**:
  - Image slider
  - Featured Product section with the product title below the image
  - All collections section
  - Newsletter signup section
- **Footer Includes**:
  - Quick links menu (search, contact, return policy, privacy policy)
  - Follow us menu (Twitter, Facebook, Pinterest, Instagram)
  - Store location map (Algonquin College address)
