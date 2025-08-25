# Episode 10 – Deploy Web App with Jenkins and NGINX

This episode demonstrates how to build a real CI/CD pipeline that:
- Pulls code from GitHub
- Automatically updates an NGINX web server on new commits
- Simulates a production-style deployment on your local home lab

#  Tools Used
- Jenkins (pre-installed)
- NGINX (running on port 80)
- GitHub (public repo with personal access token)

##  Pipeline Logic
1. Clone GitHub repo into Jenkins workspace
2. Copy index.html to /var/www/html
3. Refresh browser to verify changes

##  Setup Steps
1. Create GitHub repo and add index.html
2. Make sure Jenkins has access to /var/www/html
3. Configure credentials and pipeline in Jenkins
4. Trigger build, verify success

##  Permissions
Ensure Jenkins can write to `/var/www/html`:
```bash
sudo chown -R jenkins:jenkins /var/www/html
sudo chmod -R 755 /var/www/html
```

##  Update Flow
1. Modify `index.html`
2. `git add . && git commit -m "Update"`
3. `git push origin main`
4. Trigger Jenkins build

##  Share
Tag your builds, share your screenshots and tell us what broke—and how you fixed it.
