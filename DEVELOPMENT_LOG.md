# -----------------------------------------------
# 1. Project Files (OS/IDE)
# -----------------------------------------------
.DS_Store
.idea/
.vscode/
Thumbs.db
*.bak
*.swp

# -----------------------------------------------
# 2. Dependency Directories
# -----------------------------------------------
/vendor/
/node_modules/
/bower_components/

# -----------------------------------------------
# 3. WordPress/WooCommerce Specific (CRITICAL)
# -----------------------------------------------
# Do not track local wp-config.php containing DB credentials
/wp-config.php
/.env
.env.local

# Debugging and Logging
*.log
/debug.log
/error.log
/sitemap*.xml
/sitemap*.xml.gz

# Ignore entire development directories if you only track the plugin itself
/wp-content/cache/
/wp-content/uploads/
/wp-content/upgrade/

# -----------------------------------------------
# 4. WordPress Standard Plugins (Ignore local build files)
# -----------------------------------------------
*.zip
*.tar
*.gz
/assets/dist/
/build/
4. Commit the File
Scroll down and click "Commit new file."

This list is better than the basic templates because it includes the necessary files for the PHP, JavaScript, and WordPress environments all in one place, ensuring maximum safety for your sensitive files (.env, wp-config.php).

Now you are truly ready to push your local code!
