# IsaacLab-Hello-World

# 0- Pre-Requisites
Make sure you have IsaacSim and IsaacLab installed and your Python environment created with Anaconda Prompt. If you haven't check: https://github.com/marcelpatrick/IsaacSim-IsaacLab-installation-for-Windows-Easy-Tutorial/blob/main/README.md 
 

# 1- Activate Conda Environment
. Open Anaconda Prompt Terminal
. From base path run ``conda activate [YOUR ENV NAME]`` in this example ``conda activate env_isaaclab``

# 2- Run Internal Projects
. Run projects that come with the IsaacSim template project cloned from GitHub
. Navigate to ```C:\Users\[YOUR USER]\IsaacLab```

. Run Internal Project demos available in the repo:
```
python scripts\tutorials\05_controllers\run_diff_ik.py
python scripts\tutorials\01_assets\run_deformable_object.py
python scripts\tutorials\02_scene\create_scene.py
python scripts\tutorials\03_envs\create_quadruped_base_env.py
isaaclab.bat -p scripts\demos\h1_locomotion.py
```

# 3- Run External Projects

## 3.1- Pre-Requisites
Create an external project. If you haven't, check: https://github.com/marcelpatrick/create-a-new-external-isaaclab-project/blob/main/README.md

. Navigate to: ``(env_isaaclab) C:\Users\[YOUR USER]\[YOUR PROJECT NAME]`` in this example: ``(env_isaaclab) C:\Users\[YOUR USER]\MyIsaacLabProject``

## 3.2- Running a Task Already in Your Project (Cartpole)
- When we create an external project using [Template Generator](https://github.com/marcelpatrick/create-a-new-external-isaaclab-project/blob/main/README.md), it is created with one template simulation task: Cartpole
- Here we will run the Cartpole task with its default training and reward function parameters. 
- In Anaconda Prompt terminal, inside your env root folder, run the cartpole task `python MyIsaacLabProject/scripts/rsl_rl/train.py --task=Template-Myisaaclabproject-v0`


