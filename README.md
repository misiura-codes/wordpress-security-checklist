# WordPress Security Checklist

## 1. Preparation and Backup

- [ ] **Backup Your Site**: Create a full backup of your files and database. This ensures you can restore your site if anything goes wrong during the cleanup process.

## 2. Initial Scan and Analysis

- [ ] **Initial Scan with WordFence**: Scan your website with WordFence to identify available updates and potential malware.
- [ ] **Download Site Files**: Download all your site files to your computer or server.

## 3. Cleanup Process

- [ ] **Remove Unnecessary Files**: Delete all WordPress core files, suspicious files, plugins, and themes, but keep `wp-content/uploads/` and `wp-config.php`.
- [ ] **Secondary Scans**: Scan the remaining files with additional tools like ImunifyAV and Malcure for thorough malware detection.
- [ ] **Manual File Check**: Manually inspect all remaining files, especially `.php`, `.js`, and `.htaccess` files, for any suspicious code.
- [ ] **Database Check**: Examine your database dump for any suspicious links or scripts.
- [ ] **Review Plugins and Themes**: Go through the list of installed plugins and themes, removing any that are unnecessary or unused.

## 4. Reinstallation and Upload

- [ ] **Download Clean Versions**: Get the latest clean versions of all your themes, plugins, and WordPress core files.
- [ ] **Upload Clean Files**: Upload the cleaned files back to your server. Consider using a new cPanel account if you manage multiple websites.

## 5. Security Enhancements

- [ ] **Update Admin Passwords**: Change all WordPress admin passwords directly via the database.
- [ ] **Check cPanel**: Inspect cPanel for any suspicious activity such as unauthorized FTP accounts, email accounts, cron jobs, SSH keys, and cPanel contact email. Change passwords as needed.
- [ ] **Remove Old Files**: Delete any old or unnecessary files and perform another full server scan, including the full cPanel, not just the `public_html` folder.
- [ ] **Update wp-config.php**: Change the salts and update database credentials in `wp-config.php`.
- [ ] **Purge Cache**: Clear the website cache to ensure all changes are applied.

## 6. Post-Cleanup Verification

- [ ] **Website Functionality Check**: Ensure your website is functioning correctly after the cleanup.
- [ ] **Install Simple History**: Install the Simple History plugin for tracking changes and activity on your site.
- [ ] **Configure Security Plugin**: Set up WordFence or another security plugin to provide ongoing protection.
- [ ] **WP-CLI Check**: Use WP-CLI to check plugins and WordPress core files for any issues.
- [ ] **Final Scan with WordFence**: Perform another scan with WordFence to ensure the site is clean.
- [ ] **Blacklist Check**: Verify your domain against blacklists using VirusTotal and Urlvoid. Submit removal requests if needed.
- [ ] **Create Clean Backup**: Make a new backup of your now clean website.

## 7. Final Steps

- [ ] **Check SSL Certificates**: Ensure your SSL certificates are correctly installed and up-to-date.
- [ ] **Enable Auto Updates**: Enable automatic updates for WordPress core, themes, and plugins to keep everything up-to-date.
