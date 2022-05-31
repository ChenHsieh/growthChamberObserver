# growthChamberObserver

I got a summer research grant for 2022 from graduate school of UGA. I am working on a project to observe the growth of Arabidopsis thaliana in growth chamber with raspberry pi and other fun cameras. I am using AWS IoT to communicate with the raspberry pi.

## command

to activate the monitoring

```bash
python3 humiditySensor.py --endpoint my_end_point.iot.us-east-1.amazonaws.com --rootCA ~/certs/AmazonRootCA1.cer --cert ~/certs/cert.stuff.pem.crt --key ~/certs/private.key --thingName RaspberryPi001 --clientId RaspberryPi001
```

I set up SNS service that would send me an email when the temperature is over 80˚F.