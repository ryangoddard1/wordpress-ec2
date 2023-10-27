<H2>Hosting a Wordpress site via Apache web server on AWS EC2 w/ subdomain</H2>
<p>I wanted this to serve as the first instance in a larger scale Terraform project. This project runs an EC2 instance on an Ubuntu server (22.04). Putty was used to SSH to the server to run basic updates, install Apache web server, MySQL & WordPress with associated users/permissions, configuring the default.conf file in /apache/, to finishing off with deploying HTTPS w/ Certbot</p>

<h4>Architecture / Flowchart</h4>

![ec2-wordpress2](https://github.com/ryangoddard1/wordpress-ec2/assets/84172786/00d65123-fad6-4823-b8ee-334cb3a161b5)


<h4>Apache default.conf server settings</h4>

![nanoconf](https://github.com/ryangoddard1/wordpress-ec2/assets/84172786/f06522a0-9ce7-442c-941a-dd5864e2b7cc)


<h4>WordPress pointing to subdomain URL w/ TLS via Let's Encrypt</h4>

![wp-admin](https://github.com/ryangoddard1/wordpress-ec2/assets/84172786/5cccc761-b0b2-46d6-9069-64823303b18d)

<h4>Update 10/27</h4>
<p>Verified able to restore EC2 Instance via EBS Snapshot saved as AMI
Attempted creating gallery via WP - received “Is its parent directory writable by the server?
Remedied by SSH'ing to server
cd /var/www/html/wordpress/wp-content
mkdir uploads (wasn't present)
chown -R www-data:www-data uploads (permissions)
chmod 755 -R uploads (permissions)
sudo systemctl restart apache2 (reload to take effect)
Verified able to upload dog pics</p>

![image](https://github.com/ryangoddard1/wordpress-ec2/assets/84172786/b216d4ae-9e56-4536-a55a-f4fe677def14)



<h4>Services / Utilities:</h4>
  <ul>
  <li>EC2</li>
  <li>SSH</li>
  <li>Ubuntu CLI</li>
  <li>WordPress</li>
  <li>Route 53</li>
  </ul>
