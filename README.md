# Summary: 

I live fairly close to the water in the East Bay, and my home is always very humid ( > 60% pretty consistently).  Some areas, such as the closets and garage, have begun to show some signs of mold growth.

To help address this, I'm planning to place a few Raspberry Pi Zero 2 W's + humidity sensors (connected via GPIOs) in different areas of my home to monitor the humidity level.  These will then transmit that data directly to a database (MongoDB), which will be connected to a web-front end to view the collected data.

## Considerations
* How often to sample + transmit data.  e.g. 1 sample/sec or 1 sample/min
* Historical data / metrics  - calendar interface to select a particular date or range of dates
    * Max humidity in date range
    * Min humidity in date range
    * Average humidity in date range

## Other features I'm considering:
* Adding a messaging (email or sms) / notification service for when humidity exceeds a certain threshold
* Pull in current + historical weather information (outside temperature + humidity) via an API