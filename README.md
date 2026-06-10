# IsaacLab-Hello-World

# 0- Pre-Requisites
Make sure you have IsaacSim and IsaacLab installed and your Python environment created with Anaconda Prompt. If you haven't, check: https://github.com/marcelpatrick/IsaacSim-IsaacLab-installation-for-Windows-Easy-Tutorial/blob/main/README.md 
 

# 1- Activate Conda Environment
. Open Anaconda Prompt Terminal
. From base path run ``conda activate [YOUR ENV NAME]`` in this example ``conda activate env_isaaclab``

# 2- Run Template Simulation Tasks
. Run template tasks that come inside the IsaacSim template project cloned from GitHub (internal project)
. These tasks don't yet train the robots (no reinforcement learning workflow behind them). These scripts just demonstrate opening IsaacSim and running a virtual simulation: renders an environment, moves robotcs or assets around etc. Still no training. 

. Navigate to ```C:\Users\[YOUR USER]\IsaacLab```

. Run template task demos available in the repo:
```
python scripts\tutorials\05_controllers\run_diff_ik.py
python scripts\tutorials\01_assets\run_deformable_object.py
python scripts\tutorials\02_scene\create_scene.py
python scripts\tutorials\03_envs\create_quadruped_base_env.py
isaaclab.bat -p scripts\demos\h1_locomotion.py
```

# 3- Run Template Reinforcement Learning Tasks

:: Cartpole — balance a pole on a cart  
`isaaclab.bat -p scripts\reinforcement_learning\rsl_rl\train.py --task=Isaac-Cartpole-v0`

:: Ant — quadruped learning to walk forward  
`isaaclab.bat -p scripts\reinforcement_learning\rsl_rl\train.py --task=Isaac-Ant-v0`

:: Humanoid — bipedal MuJoCo-style figure learning to run
`isaaclab.bat -p scripts\reinforcement_learning\rsl_rl\train.py --task=Isaac-Humanoid-v0`

. You can also run them headless so that you only have the RL workflow running, without opening the 3D simulation on IsaacSim:
`isaaclab.bat -p scripts\reinforcement_learning\rsl_rl\train.py --task=Isaac-Cartpole-v0 --headless`

# 3- Run External Projects

## 3.1- Pre-Requisites
Create an external project. If you haven't, check: https://github.com/marcelpatrick/create-a-new-external-isaaclab-project/blob/main/README.md

. Navigate to: ``(env_isaaclab) C:\Users\[YOUR USER]\[YOUR PROJECT NAME]`` in this example: ``(env_isaaclab) C:\Users\[YOUR USER]\MyIsaacLabProject``

## 3.2- Running a Task Already in Your Project (Cartpole)
- When we create an external project using [Template Generator](https://github.com/marcelpatrick/create-a-new-external-isaaclab-project/blob/main/README.md), it is created with one template simulation task: Cartpole
- Here we will run the Cartpole task with its default Reinforcement Learning parameters. 
- In Anaconda Prompt terminal, inside your env root folder, run the cartpole task `python MyIsaacLabProject/scripts/rsl_rl/train.py --task=Template-Myisaaclabproject-v0`

# 4- Next Steps
- After this, you can go to the next level, add new tasks to your project and customize their reward function and training parameters. Check: https://github.com/marcelpatrick/Custom-IsaacLab-Manager-based-External-project 
