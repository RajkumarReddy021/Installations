## Debug Stops for AIrflow
# Firewall wall checks
  sudo ufw allow 8080   
  sudo iptables -A INPUT -p tcp --dport 8080 -j ACCEPT 
# Check for Port Conflicts 
  sudo lsof -i -P -n | grep LISTEN 
