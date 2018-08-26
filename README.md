Coming Soon Page with Video Background and Subscription Form
============================================================
CSoon is a Bootstrap 4 coming soon theme featuring video background and the subscription form perfect to act as your landing page for a project that is under construction.
    
    Designed by Start Bootstrap
    https://startbootstrap.com/template-overviews/coming-soon
    
    Adapted for OctoberCMS by NRuslan.
    https://nruslan.com
    
Required plugin: Drivers http://octobercms.com/plugin/october-drivers

### Installation and Configuration Steps
1. Install the theme and make it active.
2. Install OctoberCMS plugin
3. Update the plugin (How to update: Navigate your terminal to `~\[OctoberCMSfolder]\plugins\october\drivers`, type `composer update` and press enter.)
4. In the mail configuration file which is located `config\mail.php`, change your driver to mailgun `'driver' => 'mailgun'`.
5. Go to the backend of your OctoberCMS website and navigate to mail configuration page `http://yourWebsite.co/backend/system/settings/update/october/system/mail_settings` and specify your Mailgun domain and Mailgun secret which is Mailgun private API key.
6. Create a new mail template in `http://yourWebsite.co/backend/system/mailtemplates` with the email variable. (Check the email example below)
7. Now you need to define your email template that has been created in the step 6 in `~\[OctoberCMSfolder]\themes\csoon\pages\index.htm` like so `Mail::send('emailTemplate::code', $data, function($message){}`, and specify your valid email box.
> **Email Example**:
    
    I want to get a notification when your website will be up.
    My email is {{ email }}.
    Thank you!
    
If you want to use a different background video the link is located at `themes\csoon\layouts\default.htm`

