# Galaxy
This game is basic one which involves the piece on the screen navigating through the path in space.

# Installation
To install the game, it is best to create a virtual environment and to run in vs code. To install a virtual environment in vs code execute the command in vs code's terminal
'''
python --m venv virtual_env
'''
and put all the files and folders into the folder of the virtual environment. 
The next thing is to install the required version of Kivy library. To install Kivy-2.3.0 for cpython 3.8 install the file Kivy-2.3.0-cp38-cp38-win_amd64.whl for windows x64.
Execute the command
pip install Kivy and it will install the kivy library

# Basic game logic
The classes imported for the game would be kivy.config.Config for configuring the settings of the game window and kivy.core.audio.SoundLoader which is for adding sounds into the game. Some more classes imported would be the kivy.lang.Builder, kivy.core.window.Window, kivy.uix.relativelayout.RelativeLayout, kivy.platform, kivy.app.App, kivy.properties, kivy.graphics.context_instructions, vertex_instructions.

The first part starts by building the screen of the game and for that we are setting its size to (900, 500). 
'''
Config.set('graphics', 'width', '900')
Config.set('graphics', 'height', '500')
'''
In the game we have defined various variables like perspective_point_x, perspective_point_y which actually are used in the game to help trace out the path. menu_widget is the ObjectProperty variable that is used for linking the menu.kv file to the main.kv and also obtain the functionality. vertical_lines is the list of vertical lines of the path and horizontal_lines is for horizontal lines in the path. We use 8 vertical lines and 10 horizontal lines. The spacing set between vertical lines is 0.2 and between horizontal lines is 0.1. current_offset_x is the offset of the vertical lines on the screen in the x direction and current_offset_y is the offset of the vertical lines in the y direction. Another important component is the tiles list which contain the tiles or the coordinates of the intersection of the horizontal and vertical lines. current_loop_y is the main variable that allows the horizontal f

# Initialization function
We initialize everything from sounds in the game to the 


