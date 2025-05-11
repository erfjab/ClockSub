![Preview](preview.png)

## Marzneshin [server]

1. **Download the template:**
   ```sh
   sudo wget -N -P /var/lib/marzneshin/templates/subscription/ https://raw.githubusercontent.com/erfjab/ClockSub/refs/heads/main/marzneshin/index.html
   ```

2. **Run these commands:**
   ```sh
   echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzneshin/templates/"' | sudo tee -a /etc/opt/marzneshin/.env
   echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /etc/opt/marzneshin/.env
   ```
   Or uncomment these lines in `/etc/opt/marzneshin/.env`:
   ```
   CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzneshin/templates/"
   SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
   ```

3. **Restart Marzneshin:**
   ```sh
   marzneshin restart
   ```

## Marzneshin [host]

check and use:

```bash
https://raw.githubusercontent.com/erfjab/ClockSub/refs/heads/main/marzneshin/marzneshin.php
```