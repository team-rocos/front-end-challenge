# front-end-challenge

The objective of this challenge is to demonstrate live telemetry data flowing from the Rocos platform to a custom web frontend.

The specific visuals should include a horizon and heading gauge. They can be simple but need to show roll, pitch, yaw in a graphic format.

Here is an example (the first gauge): https://aviation.stackexchange.com/questions/35933/what-is-the-exact-meaning-of-attitude-does-it-include-translational-movement

The simulated telemetry data is provided by a virtual robot running on Rocos platform. This virtual robot is named `drone-rocos` within project `front-end-challenge` and the telemetry data is available at data url `/mavlink/ATTITUDE` with the data format below. 

```
{
  "pitch": -0.20733291,
  "pitchspeed": 0.10963227,
  "roll": 0.009296797,
  "rollspeed": -0.009649444,
  "time_boot_ms": 1482066,
  "yaw": 1.5808406,
  "yawspeed": -0.0020616255
}
```


Once complete, please send a link to the code via a GitHub repository.  

We are not worried about it looking pretty.

The reason this is important to Rocos is that we have live connections to autonomous robots showing a range of telemetry information in live frontend interfaces.


## Time:

Ideally only around 2 hours is spent on the core task.  Suggest keeping the design to a minimum not to take up too much time.  Some research time before hand may be required on streaming technology like RxJS or upskilling on Angular to build a simple application, services and components.

## Preparation
- You can find the Rocos JS SDK documentation from https://sdk.rocos.io/js/docs/.
- You can play the demo application located within `./demo` folder. (The demo project id is `front-end-challenge`)
- You can email `jing.li@rocos.io` to request the `Application ID` and `Application Secret` for running the demo application and building your application.

## Tech stack:
- Angular (Latest version 10+)
- RxJS Observables with Rocos JS SDK (demonstrate use of our streaming data)
- Each gauge should be an angular component
