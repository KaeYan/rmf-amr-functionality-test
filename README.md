# AMR Functionality Test (Step 3)

To perform door request, lift request and robot loop request 

### Door requests
	source /opt/ros/foxy/setup.bash
  	source <company_name>_ws/install/setup.bash
  	python3 ~/AMR_S3_FuncTest_ws/src/functionality_test/functionality_test/test_door_request.py \
		<door_name> <requested_id> <door_mode>
	# door mode: MODE_CLOSED = 0; MODE_MOVING = 1; MODE_OPEN = 2; MODE_OFFLINE = 3; MODE_UNKNOWN = 4
		
### Lift requests
	source /opt/ros/foxy/setup.bash
  	source <company_name>_ws/install/setup.bash
  	python3 ~/AMR_S3_FuncTest_ws/src/functionality_test/functionality_test/test_lift_request.py \
		<lift_name> <session_id> <request_type> <destination_floor> <door_state>
	# request type: REQUEST_END_SESSION = 0; REQUEST_AGV_MODE = 1; REQUEST_HUMAN_MODE = 2
	# door_state: DOOR_CLOSED = 0; DOOR_OPEN = 2
	
### Loop requests
	source /opt/ros/foxy/setup.bash
  	source <company_name>_ws/install/setup.bash
  	python3 ~/AMR_S3_FuncTest_ws/src/functionality_test/functionality_test/test_loop_request.py \
		<start_name> <finish_name> <robot_type> <num_loops>
		

