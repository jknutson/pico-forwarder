# pico-forwarder

## Usage

Options:

```
Usage: forwarder [options]
        Read data from Serial port and emit to MQTT
        Options:
  -mqBroker string
        MQ Broker (Host) (default "tcp://localhost:1883")
  -mqClientID string
        MQ Client ID (default "pico-forwarder")
  -mqTopic string
        MQ Topic Base (default "pico-forwarder")
  -serialBaud int
        baud rate (default 115200)
  -serialPort string
        path to serial port (default "/dev/ttyACM0")
  -verbose
        verbose output
  -version
        show version
For more information, see https://github.com/jknutson/pico-forwarder
```

Example:

```
./pico-forwarder -mqBroker tcp://mqtt.contoso.com:1883 -mqTopic pico-forwarder -serialPort /dev/tty.usbserial-0001
```
