# `level-0`

Welcome to Level Zero's GitHub Classroom!

This level is where contributors who are unfamiliar with the project should
start. Contributions at this level can be made by pointing out inconsistensies,
errors or other such problems in existing tutorials and documentation. This can
be done by creating issues in the repository using the correct issue templates.

This tutorial will teach you how to setup and run a model using the framework,
as well as how to set up their environment for development.

## Instructions

### 1. Run the `setup` script

```sh
# ./setup
```

The setup script will download the starter code for the predator-prey model for
you into the `model/` folder.

### 2. Run the model

To run the model, move into the `model/` folder, install all dependencies, and
pass the configuration to the `main.py` file as follows:

```sh
# cd model/
# pip install -r requirements.txt
# python main.py -c config.yaml
```

Upon running the model, a `.gif` file will be generated in the `media/` folder,
called `predator-prey.gif`. It will contain an animation of the predators' and
prey's movements for all the steps in the single episode that is executed.

### 3. Make some changes

For example, try increasing the number of steps in one epoch/episode by opening
the `config.yaml` file and changing the value of `num_steps_per_episode` to
`96`. Then, re-run the simulation as shown in step two.

### 4. Push your changes

After viewing the updated `.gif`, `git push` your changes to complete the
assignment.
