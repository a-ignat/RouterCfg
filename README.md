# RouterCfg

This is an SSH/Telnet client created in python and designed to connect to network devices and send commands.
Devices are specified by user in a separate file and so do commands.
The set of commands are sent to all devices.
User must also provide username and password with full access to devices.

Each device is created in a separate thread, only if preliminary checks are passed. If not it is proceeded to the next device. Commands are executed one by one and their output is kept in Router.output field. Errors while executing command on device are displayed, but do not cause the script to abort. This may be changed to your liking.

Script can be interrupted by user, pressing Ctrl + c at keyboard.
