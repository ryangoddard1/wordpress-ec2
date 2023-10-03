<H2>Hosting a Wordpress site via Apache web server on AWS EC2 w/ subdomain</H2>
<p>I wanted this to serve as the first instance in a larger scale Terraform project. This project runs an EC2 instance on an Ubuntu server (22.04). Putty was used to SSH to the server to run basic updates, install Apache web server, MySQL & WordPress with associated users/permissions, configuring the default.conf file in /apache/, to finishing off with deploying HTTPS w/ Certbot</p>


<h4>Apache default.conf server settings</h4>
![image](https://github.com/ryangoddard1/wordpress-ec2/assets/84172786/2ac58298-f899-4c4a-a4e9-56599bfd3f19)

<h4>WordPress pointing to subdomain URL w/ TLS via Let's Encrypt</h4>
![image](https://github.com/ryangoddard1/wordpress-ec2/assets/84172786/594cab18-2984-4c23-b07a-f9d04f94b94c)


<h4>Services / Utilities:</h4>
  <ul>
  <li>EC2</li>
  <li>SSH</li>
  <li>Ubuntu CLI</li>
  <li>WordPress</li>
  <li>Route 53</li>
  </ul>
