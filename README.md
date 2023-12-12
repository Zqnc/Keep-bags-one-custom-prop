# Keep-bags-one-custom-prop
This script is from https://github.com/swkeep/keep-bags and this is some custom made for fun.

#1. step download keep-bagsV2






#2. step is go in files keep-bags/shared/props 
and add this lines below backpack2

backpack3 = {
        dict = 'amb@world_human_hiker_standing@female@base',
        anim = 'base',
        bone = 'bag',
        attaching_position = {
            x = -0.00,
            y = -0.00,
            z = -0.00,
            xRotation = 0.0,
            yRotation = 00.0,
            zRotation = 0.0,
        }
    },

![image](https://github.com/Zqnc/Keep-bags-one-custom-prop/assets/153567846/594b94ee-03c8-4403-b82f-2395a9645213)


#3. Next one is go to keep-bags/config and below follow the photo:
![Uploading image.png…]()


{
          item = 'backpack3',
          slots = 20,
          size = 50000,
          prop = GetProp('backpack2') -- Use props from shared/props.lua
     },

