# EmailJS Setup Guide

## 🚀 Complete Setup Instructions

### 1. Create EmailJS Template

1. Go to [EmailJS Dashboard](https://dashboard.emailjs.com/)
2. Click on **"Email Templates"** in the sidebar
3. Click **"Create New Template"**
4. Use this template content:

**Subject:** New Contact Form Submission from {{from_name}}

**Content:**
```
Hello Vighnesh,

You have received a new message from your portfolio contact form:

From: {{from_name}}
Email: {{from_email}}

Message:
{{message}}

---
Sent from your portfolio website
```

5. Save the template and copy the **Template ID**

### 2. Get Your Public Key

1. In EmailJS Dashboard, go to **"Account"** → **"General"**
2. Copy your **Public Key**

### 3. Update Environment Variables

Update your `.env.local` file with:

```env
NEXT_PUBLIC_EMAILJS_SERVICE_ID=service_smb9fxv
NEXT_PUBLIC_EMAILJS_TEMPLATE_ID=your_template_id_here
NEXT_PUBLIC_EMAILJS_PUBLIC_KEY=your_public_key_here
```

Replace:
- `your_template_id_here` with your actual Template ID
- `your_public_key_here` with your actual Public Key

### 4. Test Your Form

1. Restart your development server: `npm run dev`
2. Fill out the contact form on your website
3. Check your email inbox for the message!

## 📧 Email Template Variables

The template uses these variables:
- `{{from_name}}` - User's full name
- `{{from_email}}` - User's email address  
- `{{message}}` - User's message
- `{{to_name}}` - Your name (Vighnesh Bhati)

## 🔧 Troubleshooting

If emails aren't working:
1. Check browser console for errors
2. Verify all environment variables are set correctly
3. Make sure your EmailJS service is connected to your email
4. Check EmailJS dashboard for failed sends

## 📊 EmailJS Free Tier

- 200 emails per month
- No credit card required
- Perfect for portfolio contact forms