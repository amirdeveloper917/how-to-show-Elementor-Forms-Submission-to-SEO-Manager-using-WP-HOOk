# how-to-show-Elementor-Forms-Submission-to-SEO-Manager-using-WP-HOOk
This article shows how you can give your SEO leads access to Elementor form submissions without giving them full admin privileges. I’m currently using this snippet myself and wanted to share it so others can save time and avoid unnecessary hassle.


It also ensures that your SEO team cannot access other Elementor pages, templates or sensitive plugin pages. The snippet works whether you’re using Yoast SEO or just the default WordPress editor.

**What It Does**

Form Submissions Access
Allows selected roles to view and export Elementor form submissions.

**Roles included:**
wpseo_manager
wpseo_editor
editor

Block Other Elementor Pages

Only the Form Submissions page is accessible.

All other Elementor pages and submenus are blocked for these roles.

**Hide Elementor Submenus**

Removes unnecessary Elementor menu options for the selected roles.
Block Plugin Pages
Blocks access to other plugin pages that are sensitive, such as:
WP File Manager
UpdraftPlus
WP Mail SMTP
All-in-One WP Migration
Hide Elementor Templates

Prevents access to Elementor templates through both menus and direct URLs for SEO roles and Editor.

**Yoast SEO Access**

Provides full Yoast access for SEO roles.
Does not give full WordPress admin rights.
Roles & Permissions
Role	Access	Notes
wpseo_manager	Elementor Form Submissions + Yoast	Other Elementor pages/templates blocked
wpseo_editor	Elementor Form Submissions + Yoast	Same restrictions
editor	Elementor Form Submissions	Cannot access blocked pages/templates
Admin	Full access	No restrictions

**How to Use**

Add this snippet to a custom plugin or your child theme’s functions.php.
Make sure the roles exist (wpseo_manager, wpseo_editor) or create them.

Test by logging in as an SEO role to confirm:
Form Submissions are visible
Other Elementor pages/templates are hidden
Plugin pages like File Manager are blocked
Yoast SEO dashboard accessible

Now enjoy ..

