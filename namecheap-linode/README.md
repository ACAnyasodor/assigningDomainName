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
- For each record, add the IPv4 and IPv6 address as the IP address, leave **_Hostname_** empty and leave TTL as default; save
### Namecheap/Domain Settings
- Open the domain dashboard
- Set **_Nameservers_** to **_Custom DNS_**
- Add **_ns1.linode.com_** till **_ns5.linode.com_** to Nameservers
- Save  

You'll have to wait a while for the changes to take effect. According to articles I read during my research, it should take a maximum of 24 hours. It is usually faster in some cases.
