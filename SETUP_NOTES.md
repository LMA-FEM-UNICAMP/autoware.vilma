# How to setup the workspace

## Autoware launcher config dir

In vehicle section, change 

```
<arg name="config_dir" value="$(find-pkg-share individual_params)/config/$(var vehicle_id)/$(var sensor_model)"/>
```

with

```
<arg name="config_dir" value="$(find-pkg-share $(var sensor_model)_description)/config"/>
```