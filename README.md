# macaddresschanger
It changes the mac address to a rogue mac address
import subprocess
subprocess.call("ifconfig", shell="True")
subprocess.call("ifconfig en0 down", shell="True")
subprocess.call("ifconfig en0 hw ether 00:11:22:33:44:55", shell="true")
subprocess.call("ifconfig en0 up", shell="True")
