# AMR Functionality Test (Step 3)

To perform door request, lift request and robot loop request 

### Door requests
	source /opt/ros/foxy/setup.bash
  source <company_name>_ws/install/setup.bash
  python3 ~/AMR_S3_FuncTest_ws/src/functionality_test/functionality_test/test_door_request.py <door_name> <requested_id> <door_mode>
