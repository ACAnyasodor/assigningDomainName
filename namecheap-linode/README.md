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
### Namecheap/Domain Settings
- Open the domain dashboard
- Set **_Nameservers_** to **_custom DNS_**
- Add **_ns1.linode.com_** till **_ns5.linode.com_** to Nameservers
- Click ![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJgAAACYCAMAAAAvHNATAAAAjVBMVEX///8ClkIAlD3//f8AkTQAjy8AjywAlDgAlTwAkjj8//4AkSoAjCMAkzPx+vVIp2ba69/F4s82oVoAiQtms3v3+PmNxZ5ApGDP6NgimEuh0bRVrXM0oFF3vo/1+viPxaOw3L2CxJibzquZyKnZ8eG838hxuYay2b/k8+gnmkZgrXFws4RktoNStXYfoFTUOD1eAAAC1klEQVR4nO3ZXZOaMBQG4JwIAQJBsBZBlO3a4rKr3f//80oQWKH7cVWS6bzPpY7DOyfJSYKMAQAAAAAAAAAAAAAA/AfiJDYd4V3p5tv2u+kQMyvGqszzgp1tJZMs3whSRa4j2qMNs+cOOYeEraTpMBNJGRGJF7vGsS1RflCc3DK2bBxlJnhbr6Nkdg1jdQy7XJXpIDOJr4gofDCdY6Iduh/UlouLR9NRZqos4rpeJ9NBZuTV8XW9MtNBZpKdIF2vn6aDTEj26+DocbRuftWF39XLtnGsu3KRuJoOMrMPulzh2a79ke1Fl0sd7Or38sHTscjbNaaj3FuxU9dWiavErn375HT14l5tOsnUKepicbE3nWSqrxeJs+kkU/volstZ27Ugn27rkbhv1YIc+n2bq15wQVas+eJhOb/lWvjEWpXRJf6sEPlzn8stl0vVag5cbPKPv483w0AWybI3tVoQj04frbaqdKnvFIt31of2SBqWHxwYjqJfkO5VLrwTSZa1D1f0d0Hk0PB1sN3iHay9S5chke+9s9mkQZ+LXCNbZLzWAcLL/D1EE/lDLkNn/MTVCcR2OtGql36HJJ8aE6+a2kemXU9Qh+T+80s4DKSzZMu/t2JZF8Ip7jpaLYZcXmnqaNg+d90NG3fGSZ4TH1ZkYHLvTm47j8fT/oNNMM58s7fIWr2dndsKZuNActNvpc9uf7jRb6FTf6gXRU9mc7G4uE0q/zln1TjBDM78nmR71TeHQ5ONnYKC9Ovf/mvrfgcKijEWKRuuH+lwxBnHkbhoLLjfri4OzagjW/q4856cz4M9J1//aglHd5rLseXNYRxMcvmuDTNMk4+TWaZsKdi4ZfYKS2aYdr6bZepiyUBqjXgLZkUPG22DYTDV1qJckqVq7PqfXNANkNvby2n9L6k9BdOqa+hwHoirXX8qt6qn36+vZWpXuQAAAAAAAAAAAAAAAAAAAOz0BxGWHqSjALl1AAAAAElFTkSuQmCC) to save
