# Deep-Convolutional-Q-Learning-Pac-Man

# Description
A classic arcade game. Move Pac Man around a maze collecting food and avoiding ghosts- unless you eat a Power Pellet, then you can eat the ghosts too!

# Actions
Pacman has the action space of Discrete(5) with the table below listing the meaning of each action’s meanings. To enable all 18 possible actions that can be performed on an Atari 2600, specify full_action_space=True during initialization or by passing full_action_space=True to gymnasium.make.

![Capture1](https://github.com/Mandar13022/Deep-Convolutional-Q-Learning-Pac-Man/assets/112116535/a38de3c2-188d-44dc-9b6d-0f753a7202a4)

# Observations
Atari environments have three possible observation types: "rgb", "grayscale" and "ram".
obs_type="rgb" -> observation_space=Box(0, 255, (210, 160, 3), np.uint8)
obs_type="ram" -> observation_space=Box(0, 255, (128,), np.uint8)
obs_type="grayscale" -> Box(0, 255, (210, 160), np.uint8), a grayscale version of the “rgb” type
See variants section for the type of observation used by each environment id by default.

# Variants
Pacman has the following variants of the environment id which have the following differences in observation, the number of frame-skips and the repeat action probability.

![Capture2](https://github.com/Mandar13022/Deep-Convolutional-Q-Learning-Pac-Man/assets/112116535/95e3bd1d-df4c-4d61-bcb3-1fc91212a56e)

Difficulty and modes
It is possible to specify various flavors of the environment via the keyword arguments difficulty and mode. A flavor is a combination of a game mode and a difficulty setting. The table below lists the possible difficulty and mode values along with the default values.

![Capture3](https://github.com/Mandar13022/Deep-Convolutional-Q-Learning-Pac-Man/assets/112116535/6e924d2e-2de7-42dc-8aaf-12658656963a)
