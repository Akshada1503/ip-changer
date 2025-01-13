import time


ip_addresses = [f"192.168.1.{i}" for i in range(1, 101)]


def change_ip(ip):
    print(f"Changing IP to: {ip}")
    
try:
    for ip in ip_addresses:
        change_ip(ip)
        time.sleep(1)  
except KeyboardInterrupt:
    print("Stopped by user.")
