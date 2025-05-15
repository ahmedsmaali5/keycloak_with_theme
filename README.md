
# Keycloak with Custom Theme

This repository provides a setup for running **Keycloak with a custom theme**, using Docker Compose. The theme includes changes to the login background image and logo.

# Step 1: Replace the following images:

login background image:
```bash
/keycloak-theme/newtheme/login/resources/img/keycloak-bg.png
```
login background image: 
```bash
/keycloak-theme/newtheme/login/resources/img/keycloak-logo-text.png
```

# Step 2: 🚀 Running the Project

1. Ensure Docker and Docker Compose are installed.
2. Open a terminal in the project directory.
3. Start Keycloak:
```bash
docker-compose -f docker-compose.yml up -d
```

# Step 3: Change Realm settings to use the "newtheme" instead of default Keycloak theme

1. Open Keycloak admin console:
http://localhost:8080/admin

2. Log in using your admin credentials.

3. Go to "Realm Settings" from the left sidebar.

4. Click the "Themes" tab.

5. Under Login Theme, select newtheme from the dropdown.

6. Click Save.

# Step 4: Test the changes

1. Open new private navigation window
2. Visit login page:
http://localhost:8080/realms/master/account/
