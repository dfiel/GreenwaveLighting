# GreenwaveLighting
Greenwave Lighting for Home Assistant.

This is a lighting component for the popular Home Assistant home automation software. I am in the process of getting this merged into mainstream Home Assistant, but in the mean time it can be found here. The master branch will contain a tested, working copy. Development branch has no such guarantee.

Place greenwave.py in .homeassistant/custom_components/light and add this to your configuration.yaml:

```yaml
light:
  - platform: greenwave
    host: XXX.XXX.XXX.XXX
    version: 3
```

The version option is the major revision of your firmware, which should be 2 or 3. If you are running Version 2, there are no extra steps. If you are running Version 3, you must press the Sync button on the gateway prior to the first launch of Home Assistant, so a token can be grabbed. Once home assistant has started, you can either press the Sync button again or wait for it to time out manually.
