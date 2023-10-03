<H2>Hosting a Wordpress site via Apache web server on AWS EC2 w/ subdomain</H2>
<p>I wanted this to serve as the first instance in a larger scale Terraform project. This project runs an EC2 instance on an Ubuntu server (22.04). Putty was used to SSH to the server to run basic updates, install Apache web server, MySQL & WordPress with associated users/permissions, configuring the default.conf file in /apache/, to finishing off with deploying HTTPS w/ Certbot</p>

<h4>Architecture / Flowchart</h4>

<h4>Apache default.conf server settings</h4>

![nanoconf](https://github.com/ryangoddard1/wordpress-ec2/assets/84172786/f06522a0-9ce7-442c-941a-dd5864e2b7cc)


<h4>WordPress pointing to subdomain URL w/ TLS via Let's Encrypt</h4>

![wp-admin](https://github.com/ryangoddard1/wordpress-ec2/assets/84172786/5cccc761-b0b2-46d6-9069-64823303b18d)




<h4>Services / Utilities:</h4>
  <ul>
  <li>EC2</li>
  <li>SSH</li>
  <li>Ubuntu CLI</li>
  <li>WordPress</li>
  <li>Route 53</li>
  </ul>
