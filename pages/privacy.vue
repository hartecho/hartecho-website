<template>
  <div class="body">
    <!-- prettier-ignore -->
    <div class="terms">
          <h1>Privacy Policy</h1>
          <h2>1. Information We Collect</h2>
          <p>We may collect and process the following information to provide and improve our services for custom-coded e-commerce store solutions:</p>
          
            <ul>
                <li><b>Personal Identification Information:</b> Name, email address, phone number, etc., which may be provided when you fill out our forms or join our waitlist.</li>
                <li><b>Web Usage Information:</b> IP address, browser type, version, and operating system, page views, website navigation paths, etc., to analyze how you interact with our site and improve your experience.</li>
                <li><b>Form Submission Data:</b> Information you provide when submitting forms on our website, such as inquiries about custom e-commerce stores or waitlist sign-ups, including phone numbers used for SMS communications.</li>
            </ul>
          
          <h2>2. How We Use Your Information</h2>
          <p>We use your information to:</p>
          
            <ul>
                <li>Provide our custom-coded e-commerce store services to you, including responding to inquiries and delivering tailored solutions.</li>
                <li>Track and manage form submissions on our website, such as contact forms or waitlist sign-ups, to ensure we can follow up effectively.</li>
                <li>Send text message (SMS) reminders or communications about your form submissions, waitlist status, or other relevant updates, based on your opt-in consent.</li>
                <li>Improve and personalize your experience on our website and services.</li>
                <li>Communicate with you, including responding to your inquiries or notifying you of important updates about our services.</li>
            </ul>
          
          <h2>3. SMS Waitlist and Form Tracking</h2>
          <p>Our website uses cookies and form tracking to monitor when you’ve filled out a form or shown interest in our services, such as filling out our client onboarding form or joining our waitlist. This information is used to determine when to send reminder messages via SMS. For example, HARTECHO LLC’s website uses cookies and form data to track when you’ve submitted a form or expressed interest in our custom e-commerce store services. This information is used to determine when to send reminder messages or waitlist updates via SMS.</p>

          <h2>4. Sharing of Your Information</h2>
          <p>We do not sell, distribute, or lease your personal information to non-affiliated third parties unless we have your permission or are required by law to do so. This excludes SMS opt-in data and consent; this information will not be shared with any third parties.</p>

          <h2>5. Security</h2>
          <p>We are committed to ensuring that your information is secure. To prevent unauthorized access or disclosure, we have implemented suitable physical, electronic, and managerial procedures to safeguard and secure the information we collect online.</p>

          <h2>6. Cookies</h2>
          <p>Our website uses cookies to enhance your experience and track interactions, such as form submissions or website navigation. Cookies are small files placed on your computer's hard drive that help analyze web traffic or let you know when you visit a particular site. You can choose to accept or decline cookies, but declining may limit your ability to use certain features of our site.</p>

          <h2>7. Google Analytics</h2>
          <p>Our website uses Google Analytics, a web analytics service provided by Google, Inc. ("Google"). Google Analytics uses "cookies", which are text files placed on your computer, to help the website analyze how users use the site. The information generated by the cookie about your use of the website (including your IP address) will be transmitted to and stored by Google.</p>
          <p>We use the data collected by Google Analytics to analyze website traffic and improve our website. Google may also transfer this information to third parties where required to do so by law, or where such third parties process the information on Google’s behalf. Google will not associate your IP address with any other data held by Google.</p>
          <p>For more information on Google Analytics and privacy, please visit <a href="https://policies.google.com/privacy" target="_blank" rel="noopener noreferrer">Google Privacy Policy</a>.</p>

          <h2>8. Location Tracking and Location-Based Services</h2>
          <p>We do not currently engage in location tracking or location-based services. If this changes in the future, we will update this policy to fully describe how that data is collected and for what purpose.</p>

          <h2>9. Links to Other Websites</h2>
          <p>Our website may contain links to other websites of interest. However, once you have used these links to leave our site, you should note that we do not have any control over that other website.</p>

          <h2>10. Changes to Our Privacy Policy</h2>
          <p>We may update this policy from time to time by updating this page. You should check this page occasionally to ensure that you are happy with any changes. Any updates will be posted on this page, and we may notify you via email or SMS if significant changes occur.</p>

          <h2>11. Contact Us</h2>
          <p>If you have any questions about this Privacy Policy, please contact us at sales@hartecho.com.</p>
      </div>
  </div>
</template>
  
  <script setup>
useSeoMeta({
  // Universal SEO
  title: "Privacy Policy || HARTECHO",
  description:
    "Learn how HARTECHO collects, uses, and protects your personal data. We prioritize transparency and security to ensure your information is handled with care.",

  // Open Graph (Facebook, Instagram, LinkedIn, WhatsApp, Discord, Slack)
  ogTitle: "Privacy Policy || HARTECHO",
  ogDescription:
    "Read HARTECHO's privacy policy to understand how we collect, use, and safeguard your data. Your privacy and security are our top priorities.",
  ogImage: "/HARTECHOLogo.webp", // Image remains in the root public folder
  ogUrl: "https://hartecho.com/privacy",
  ogType: "website",

  // Twitter/X
  twitterTitle: "Privacy Policy || HARTECHO",
  twitterDescription:
    "Your privacy matters. Read HARTECHO’s policy on data collection, security, and transparency.",
  twitterImage: "/HARTECHOLogo.webp", // Ensuring correct public path usage
  twitterCard: "summary_large_image",

  // Pinterest
  pinterestRichPin: "true",
});

// Structured Data
useHead({
  link: [
    {
      rel: "canonical",
      href: `https://www.hartecho.com/privacy`,
    },
  ],
  script: [
    {
      type: "application/ld+json",
      children: JSON.stringify({
        "@context": "https://schema.org",
        "@type": "WebPage",
        name: "Privacy Policy - HARTECHO",
        url: "https://www.hartecho.com/privacy",
        description:
          "HARTECHO's privacy policy outlines how we collect, use, and safeguard your personal information. Your privacy is important to us.",
        publisher: {
          "@type": "Organization",
          name: "HARTECHO",
          url: "https://www.hartecho.com",
          logo: {
            "@type": "ImageObject",
            url: "https://www.hartecho.com/HARTECHOLogo.webp",
            width: 500,
            height: 500,
          },
          contactPoint: {
            "@type": "ContactPoint",
            telephone: "+1-801-793-5456",
            contactType: "Customer Service",
            areaServed: "US",
            availableLanguage: ["English"],
          },
        },
        mainEntity: {
          "@type": "WebPageElement",
          name: "Privacy Policy",
          description:
            "This page details HARTECHO's privacy practices, including data collection, usage, and protection measures.",
        },
        potentialAction: {
          "@type": "ViewAction",
          target: "https://www.hartecho.com/privacy",
          name: "View Privacy Policy",
          description:
            "Understand how HARTECHO manages your data with our comprehensive privacy policy.",
        },
        breadcrumb: {
          "@type": "BreadcrumbList",
          itemListElement: [
            {
              "@type": "ListItem",
              position: 1,
              name: "Home",
              item: "https://www.hartecho.com",
            },
            {
              "@type": "ListItem",
              position: 2,
              name: "Privacy Policy",
              item: "https://www.hartecho.com/privacy",
            },
          ],
        },
      }),
    },
  ],
});

const emit = defineEmits(["hide-loading"]);
emit("hide-loading");
</script>
  
  <style scoped>
.body {
  width: 100%;
  min-height: 70rem;
  height: auto;
}

.terms {
  max-width: 1200px;
  margin: 4rem auto;
  width: 100%;
  padding: 0 2rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

h1 {
  font-family: "Poppins";
  font-size: 2rem;
  font-weight: bold;
  font-style: normal !important;
  margin-bottom: 2rem;
}

h2 {
  font-family: "Poppins";
  text-align: left;
  width: 100%;
  font-size: 1.3rem;
  font-weight: bold;
}

p {
  width: 100%;
  font-size: 1.3rem;
  margin-top: 0.5rem;
  margin-bottom: 2rem;
  text-align: left;
}

ul {
  list-style-type: disc;
  padding-left: 3rem;
  margin-bottom: 2rem;
}

li {
  font-size: 1.2rem;
  margin-bottom: 0.75rem;
}

a {
  color: blue;
}

a:hover {
  text-decoration: underline;
}
</style>