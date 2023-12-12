# Keep-bags-one-custom-prop
This script is from https://github.com/swkeep/keep-bags and this is some custom-made for fun.

1. step download keep-bagsV2






2. The step is to go into files keep-bags/shared/props 
and add these lines below backpack2

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


3. The next one is to go to keep-bags/config and follow the photo:


![image](https://github.com/Zqnc/Keep-bags-one-custom-prop/assets/153567846/80804e7d-f2f3-4bc3-adf1-57581d44bbbe)


{
          item = 'backpack3',
          slots = 20,
          size = 50000,
          prop = GetProp('backpack2') -- Use props from shared/props.lua
     },

After that go to [QB]/qb-core/shared/items and add this

backpack3                    = { name = "backpack3", label = "Backpack", weight = 15000, type = "item", image = "backpack3.png", unique = true, useable = true, shouldClose = true, combinable = nil, description = "zync custom backpack" },

THIS IS IT FOR THE CUSTOM PROP, THE SCRIPT WILL WORK WITH THIS PROP ON EVERY PED...

If you have a bad position of the bag and if you use scully_emotemenu script do this

1. Go to scully_emotemenu/data/animations/prop_emotes.lua

2. Find Label = 'Backpack',

3. Change it to this 
    {
        Label = 'Backpack',
        Command = 'backpack',
        Animation = 'nill',
        Dictionary = 'move_p_m_zero_rucksack',
        Options = {
            Flags = {
                Loop = true,
                Move = true,
            },
            Props = {
                {
                    Bone = 24818,
                    Name = 'p_michael_backpack_s',
                    Placement = {
                        vector3(0.080000, -0.140000, -0.050000),
                        vector3(0.000000, 90.000000, 175.000000),
                    },
                },
            },
        },
    },

   ![image](https://github.com/Zqnc/Keep-bags-one-custom-prop/assets/153567846/13c178ea-f6b3-48e5-9212-f217e3a30ce8)


   For this backpack, i have an inventory image
   
(PNG FORMAT FOR BACKPACK3)

        
        https://imgur.com/OtC4B3q
   

   Add this in [qb]\qb-inventory\html\images
   ![image](https://github.com/Zqnc/Keep-bags-one-custom-prop/assets/153567846/b6a01ab1-eea1-4359-ac43-a625869f3325)


Big thanks for https://github.com/swkeep/keep-bags/commits?author=swkeep for this script!
