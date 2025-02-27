
This is the `hello world` of URDF files.  URDF files are xml files that contain code for a visual model of a robot. It can be articulated.

```xml
<?xml version="1.0"?>
<robot name="myfirst">
  <link name="base_link">
    <visual>
      <geometry>
        <cylinder length="0.6" radius="0.2"/>
      </geometry>
    </visual>
  </link>
</robot>
```

We can now view this via:
```bash
ros2 launch urdf_tutorial display.launch.py model:=urdf/01-myfirst.urdf
```