.-Defanging-an-IP-Address-


Defang IP Address
🔒 A simple Python utility to "defang" IPv4 addresses for secure display (replacing . with [.]).

📖 Overview
Defanging an IP address prevents accidental hyperlinking in documents or logs, enhancing security. This repo provides multiple Python implementations for learning purposes.

original_ip = "192.168.1.1"
defanged_ip = defang_ip_replace(original_ip)  # Returns "192[.]168[.]1[.]1"

🛠 Methods
Method	Description	Performance
replace()	Uses Python's built-in string replacement	⚡ Fastest
split() + join()	Splits IP into octets and rejoins	⚡ Fast
Manual loop	Iterates through each character	🐢 Slow
