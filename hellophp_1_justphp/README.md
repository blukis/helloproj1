HelloWorldProj_1k564
====================

This is the project.

Run Locally
-----------

- First time setup:
	- Run "vagrant init" somethingsomething(?)
	- Create "vagran_dir/Homestead.yaml" from "vagran_dir/Homestead_TEMPLATE.yaml" (?)
	
- Run "vagran_dir/vagrant up"

Publish to Prod
---------------

- SSH to prod server/environment 
- Run commands:
	- git pull REPO_DIR
	- python REPO_DIR/buildMe/deploy.py "PATH_TO_TARGET_WWWDIR"

