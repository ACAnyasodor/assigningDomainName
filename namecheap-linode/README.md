## Here's a straightforward guide to assigning a namecheap domain to a linode VM  
You'll have to do some setting on both sides so lezz go

### Linode Settings
- On the your dashboard, click **_Domains_**
- Creata a domain
  - Enter the domain name and an email address
  - For **_insert default records_** select **_... from one of my linodes_** and select a linode
  - click **_Create Domain_**  

Now a domain name has been added, next connect to a Linode
- Go to your target linode and open **_Network_** tab
- copy the IPv4 and IPv6 addresses
- Go back to **_Domains_** and select the taget domain name.
- Scroll down to find A/AAAA Record and add an A/AAAA Record
- For each record leave **_Hostname_** empty and add the IPv4 and IPv6 address as the IP address, leave TTL as default and save
