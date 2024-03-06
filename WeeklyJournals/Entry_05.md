# Week 3: Prac 3 - WordPress CMS

## Learning Activities & Resources

- **Online Learning:**
  
https://www.linkedin.com/learning/wordpress-building-child-themes-3/set-up-a-local-development-environment?resume=false
https://www.linkedin.com/learning/wordpress-essential-training-22616273/creating-a-new-page?resume=false
https://www.linkedin.com/learning/learning-responsive-web-design-in-the-browser/welcome

## Estimated Hours

8 hours

## Content Insights

This week's practice involved developing a child theme, and I quickly realized that my exported files did not include themes and customizations for my local environment. To address this, I turned to the All-in-One WordPress Migration plugin, hoping it would transfer my entire site to a local setup.

However, I faced a new challenge with this solution: restrictive upload limits and a paywall for increasing these limits, set by the plugin's developers.

To overcome this issue, I manipulated the php.ini file within Docker to extend the PHP configuration limits myself. By adjusting parameters such as upload_max_filesize, post_max_size, and max_execution_time, my local WordPress can now handle the requirements of my site.

When I imported my site using the All-in-One WordPress Migration plugin, I discovered it replaced my local user account with the one from my live site. This meant I had to use my live site's login details for my local site. Although this was unexpected, I felt better prepared to work on my child theme using my live site account.

Finally, as I developed my child theme, I made several CSS customizations, enhancing the visual aspects to align with my vision. The changes included:
.site-content {
    background-color: #1f1f1f;
    color: white;
}
h1{
    color: white;
}
.site-content .ast-container {
    display: flex;
    background-color: Black;
    border-left: 2px solid white;
    border-right: 2px solid white;
    border-bottom: 2px solid white;
}
.main-header-bar-wrap {
    position: relative;
    border-bottom: 2px solid white;
}
strong{
    color: #b90000;
    font-size: larger;
}
.ast-desktop .ast-primary-header-bar.main-header-bar, .ast-header-break-point #masthead .ast-primary-header-bar.main-header-bar{
     background-color: black;
}
.main-header-menu > .menu-item > .menu-link, #astra-footer-menu > .menu-item > .menu-link{
    color: white;
}
.ast-builder-menu-1 .menu-item.current-menu-item>.menu-link, .ast-builder-menu-1 .inline-on-mobile .menu-item.current-menu-item>.ast-menu-toggle, .ast-builder-menu-1 .current-menu-ancestor>.menu-link{
    color: red;
}
.ast-mobile-header-wrap .ast-primary-header-bar, .ast-primary-header-bar .site-primary-header-wrap{
    min-height: 100px;
}
.site-below-footer-wrap{
    border-top: 2px solid white;
}
div.wpforms-container-full .wpforms-field-label{
    color: red;
}
.ast-site-identity .site-title a{
    color: red;
}
.main-header-menu > .menu-item:hover > .menu-link, #astra-footer-menu > .menu-item > .menu-link:hover{
    color: #b90000;
}


## Career/Employability/Learning Insights

This week, as I worked on creating a WordPress child theme, I learned a lot through tackling technical challenges, such as dealing with plugin restrictions and adjusting server settings. I also got hands-on with coding, making direct changes and customizing CSS, which strengthened my software development skills. These experiences have improved my technical abilities and made me more adaptable, enhancing my career prospects and showing that I can handle complex tasks and adapt to changes.