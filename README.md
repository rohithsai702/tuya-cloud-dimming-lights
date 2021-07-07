# Tuya Bulb Control #

This project is developed using Tuya SDK, which enables you to quickly develop smart devices, branded APP, cloud development project, etc.

For more information, please check Tuya Developer Click and Connect Challenge https://pages.tuya.com/develop/ClickAndConnect_TuyaDeveloper?_source=e9684c7ca6b31e7221c8420f5af94631


---
## Installation
Install or upgrade tuya-bulb-control:
```
$ pip install tuya-bulb-control --upgrade
```
<br>

Demo code:
```Python
from tuya_bulb_control import Bulb

CLIENT_ID = ''
SECRET_KEY = ''
DEVICE_ID = ''
REGION_KEY = 'in'

bulb = Bulb(
    client_id=CLIENT_ID,
    secret_key=SECRET_KEY,
    device_id=DEVICE_ID,
    region_key=REGION_KEY
)


# Turn on the bulb
bulb.turn_on()


# Turn off the bulb
bulb.turn_off()


# Turn off the light bulb after 5 minutes
bulb.set_toggle_timer(value=5)
```
<br>

## Steps to use the API:
#### Step 1: CLIENT_ID and SECRET_KEY
- Register or Login on <a href="https://auth.tuya.com" target="_blanck">Tuya</a>.
1. Create a cloud development project <a href="https://iot.tuya.com/cloud" target="_blanck">Cloud -> Project</a>.
2. After successful creation, you will receive the **Client ID** and **Secret Key**.


#### Step 2: DEVICE_ID
1. Install **Tuya Smart** app or **Smart Life** app on your mobile phone.
2. Go to <a href="https://iot.tuya.com/cloud/appinfo/cappId/device" target="_blanck">Cloud -> Link Devices</a> page.
3. Selecting a tab **Link Devices by App Account**.
4. Click **Add App Account** and scan the QR code with **Tuya Smart** app or **Smart Life** app.
5. Now you can go to devices <a href="https://iot.tuya.com/cloud/appinfo/cappId/deviceList" target="_blanck">Cloud -> Device List</a> and copy **Device ID**.
    * Notes: Try to select a your region if devices are not displayed.


#### Step 3: Request access to API calls
Go to <a href="https://iot.tuya.com/cloud/appinfo/cappId/setting" target="_blanck">Cloud -> API Group</a> and enable **Authorization management**, **Device Management** and **Device Control**.
<br>

<h3>Note:</h3>
In case of any errors , see the requirements file and install the libraries if needed.