Coming Soon Page with a Video Background and Subscription Form
============================================================
CSoon is a Bootstrap 4 "Coming Soon" theme featuring a video background and subscription form - a perfect landing page for a project that is under construction.
    
    Designed by Start Bootstrap
    https://startbootstrap.com/template-overviews/coming-soon
    
    Adapted for OctoberCMS by NRuslan.
    https://nruslan.com
    
Required plugin: Drivers http://octobercms.com/plugin/october-drivers

### Installation and Configuration Steps
1. Install the theme and make it active.
2. Install the OctoberCMS plugin.
3. Update the plugin (how to update: navigate in your terminal to `~\[OctoberCMSfolder]\plugins\october\drivers`, type `composer update` and press Enter.)
4. In the mail configuration file located at `config\mail.php`, change your driver to mailgun: `'driver' => 'mailgun'`.
5. Go to the backend of your OctoberCMS website and navigate to the mail configuration page `http://yourWebsite.co/backend/system/settings/update/october/system/mail_settings`. Specify your Mailgun Domain and Mailgun Secret, which is Mailgun's private API key.
6. Create a new mail template in `http://yourWebsite.co/backend/system/mailtemplates` with the {{email}} variable (check the email example below).
7. Now you need to define the email template that has been created in step 6 in the file `~\[OctoberCMSfolder]\themes\csoon\pages\index.htm`. Here is an example: `Mail::send('emailTemplate::code', $data, function($message){}`. Then, specify your valid email box.
> **Email Example**:
    
    I want to receive a notification when your website is up.
    My email is {{ email }}.
    Thank you!
    
If you want to use a different background video, the link is located at `themes\csoon\layouts\default.htm`.

