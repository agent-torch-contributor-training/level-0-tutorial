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

```shell
$ ./setup
```

The setup script will download the starter code for the predator-prey model for
you into the `model/` folder.

### 2. Run the model

To run the model, move into the `model/` folder, install all dependencies, and
pass the configuration to the `main.py` file as follows:

```shell
$ cd model/

# setup a virtual environment
$ python -m venv .venv/
$ . .venv/bin/activate

# install dependencies
$ pip install -r requirements.txt
$ pip install git+https://github.com/agenttorch/agenttorch

# run the model
$ python main.py -c config.yaml
```

Upon running the model, a `.gif` file will be generated in the `media/` folder,
called `predator-prey.gif`. It will contain an animation of the predators' and
prey's movements for all the steps in the single episode that is executed.

### 3. Make some changes

For example, try increasing the number of steps in one epoch/episode by opening
the `config.yaml` file and changing the value of `num_episodes` to `7`. Then,
re-run the simulation as shown in step two.

### 4. Push your changes

To complete the assignment, push your changes like so:

```sh
$ git add .
$ git commit -m 'change: `num_episodes` -> 7'
$ git push -u origin main
```

### 5. Completion!

If the autograding workflow completes successfully (you'll see a green tick next
to the commit message on the repository's page on GitHub), you have completed
the tutorial successfully. If not, and you find yourself stuck, please open an
issue
[here](https://github.com/agent-torch-contributor-training/level-0-tutorial/issues/new),
or ask for help on Slack/Discord.

Next, read the documentation (at
[lpm.media.mit.edu/docs](https://lpm.media.mit.edu/docs)) to do more with
AgentTorch! If you find any inconsistenies or errors, or wish to see an example
or tutorial added, feel free to contribute by opening an issue or pull request
over at [`AgentTorch/AgentTorch`](https://github.com/AgentTorch/AgentTorch).
