# IsaacLab-Hello-World

# Pre-Requisites
Install IsaacSim and IsaacLab: https://github.com/marcelpatrick/IsaacSim-IsaacLab-installation-for-Windows-Easy-Tutorial/blob/main/README.md 
Download 

# 0- Activate Conda Environment
From base path run ``conda activate [YOUR ENV NAME]`` in this example ``conda activate env_isaaclab``

# 1- Run Internal Projects
Run internal projects (projects that come inside the IsaacSim template folder)

Navigate to ```C:\Users\[YOUR USER]\IsaacLab```

Run Internal Project demos available in the repo:
```
python scripts\tutorials\05_controllers\run_diff_ik.py
python scripts\tutorials\01_assets\run_deformable_object.py
python scripts\tutorials\02_scene\create_scene.py
python scripts\tutorials\03_envs\create_quadruped_base_env.py
isaaclab.bat -p scripts\demos\h1_locomotion.py
```

# 2- Run External Projects

## Pre-Requisites
Create an external project: https://github.com/marcelpatrick/create-a-new-external-isaaclab-project/blob/main/README.md

Run external projects that were created as a template when the external project was created: ``python scripts/rsl_rl/train.py --task=Template-Myisaaclabproject-v0``


