Team members
Arkajyoti Misra		arkajyoti@gmail.com		@arko			
Dushyant Wadivkar	dushyantw@gmail.com		@dushyantw	
Fernando Damasio	fernandodamasio@hotmail.com	@fernandodamasio	
Frank Dzwonkowski	fdzwon@gmail.com		@fdzwon		
Yipeng Yuan		larkforsure@gmail.com		@larkforsure	


Instructions 
Clone the project repository
Install python dependencies

cd CarND-Capstone
pip install -r requirements.txt
cd ros
catkin_make
source devel/setup.sh
roslaunch launch/styx.launch

Run the simulator

Notes:
Using UDACITY VM and Native MAC, the simulator lag makes testing difficult. I had to update the server.py file with two lines of code to actually make the car move!

eventlet.monkey_patch()
sio = socketio.Server(async_mode='eventlet')

Despite that, the simulation can show the car not reacting when the lights are green or not stopping when the lights turn red as the car begins to move. I am not sure what outside of changing my computer can help fix this issue. 


