[AUTO GENERATED USING CHATGPT]
# **IPv4 Subnet Calculator**  

A simple **C++** tool for calculating subnet ranges based on **CIDR notation**. It validates IP addresses, splits a network into user-defined subnets, and displays relevant information such as:  
✅ **Network Address**  
✅ **Host Range**  
✅ **Broadcast Address**  
✅ **Reserved & Non-Usable IPs**  

## **Features**  
- 🛡 **Validates IP addresses** (warns about private & reserved addresses).  
- 🏗 **Divides an IP address into multiple subnets** dynamically.  
- 📊 **Displays subnet details in a structured format**.  
- 📜 **Supports standard IPv4 CIDR notation** (e.g., `/24, /30`).  

---

## **Installation & Usage**  

### **🔹 Compilation**  
Compile the project using **g++**:  
```sh
g++ -o subnet_calc main.cpp
```

### **🔹 Running the Program**  
Execute the compiled binary:  
```sh
./subnet_calc
```

### **🔹 Menu Options**  
```
1.) Start Subnet Calculation
2.) Show List of Non-Usable IPs
3.) Quit Program
```

---

## **Example Output**  

### **Subnet Calculation Example**  
```
Enter IPv4 address (e.g., 192.168.1.0): 10.0.0.0
Enter CIDR notation (e.g., 24 for /24): 4
Enter number of subnets to divide into: 4
WARNING: 10.0.0.0/8 is a private network. Cannot be used on public internet (RFC 1918).

New Subnet Mask: /26
-----------------------------------------------------------------------------
Subnet         Network Address   Host Range                 Broadcast Address    
-----------------------------------------------------------------------------
Subnet 1       10.0.0.0          10.0.0.1 - 10.0.0.62       10.0.0.63            
Subnet 2       10.0.0.64         10.0.0.65 - 10.0.0.126     10.0.0.127           
Subnet 3       10.0.0.128        10.0.0.129 - 10.0.0.190    10.0.0.191           
Subnet 4       10.0.0.192        10.0.0.193 - 10.0.0.254    10.0.0.255           

```

---

## **List of Reserved & Non-Usable IPs**  

| **Address**         | **Description** |
|---------------------|-------------------------------------|
| `0.0.0.0/32`       | Host address (RFC 5735) |
| `10.0.0.0/8`       | Private network (RFC 1918) |
| `127.0.0.0/8`      | Loopback address |
| `169.254.0.0/16`   | APIPA (Auto IP) |
| `172.16.0.0/12`    | Private network (RFC 1918) |
| `192.168.0.0/16`   | Private network (RFC 1918) |
| `224.0.0.0/4`      | Multicast addresses |
| `240.0.0.0/4`      | Reserved (RFC 1700) |
| `255.255.255.255`  | Limited broadcast address |

---

## **Planned Features**  
n/a unless you can come up with something useful 

---

## **License**  
This project is licensed under the **NOC License**. See the [LICENSE](LICENSE) file for details.  

## **Contributions & Contact**  
📌 Feel free to contribute via pull requests!  
📌 Report issues on **GitHub** or contact me at **ilikecirnoxd@gmail.com**.  

---
