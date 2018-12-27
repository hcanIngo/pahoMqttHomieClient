## Linux pahoMqttHomieClient                    Ingo Lages, 12/2018

### Schritte zum eigenen Mqtt-Homie-Device

1. git clone https://github.com/hcanIngo/pahoMqttHomieClient.git

2. Mqtt-Broker installieren.

3. Im Makefile BROKER_IP und BROKER_REGISTRIERUNG anpassen 

4. make installPahoLib

5. make release

6. make start

7. Pruefen z.B. per MqttLens: 
    Subscribe:  homie/#
    Subscribe:  homie/testdevice/#
    Subscribe:  homie/testdevice/$name
    Subscribe:  homie/testdevice/$state
    
8. Eigenes Devices (aehnlich test_device.h) erzeugen.

9. Anbindung an das eigene reale Device realisieren. 
