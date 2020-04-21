<h2>Motivation</h2>
given a droplet on digital ocean the question is : how can you put on it more than one web site \ web app each with its own ssl certificate and own domain name

<h2>Steps</h2>
<ol>
<li>define domains and relate to the droplet in digital ocean</li>
<li>each server app should listen on different port</li>
<li>invoke for each domain the command cerbot e.g. 
<ol>
<li>certbot --nginx -d nathankrasney.xyz -d www.nathankrasney.xyz</li>
<li>certbot --nginx -d nathankrasney.site -d www.nathankrasney.site</li>
</ol>
</li>
<li>update the correct port in /etc/nginx/sites-available/default</li>
</ol>

<h2>Sample default file</h2>
<a href="default">here</a>
