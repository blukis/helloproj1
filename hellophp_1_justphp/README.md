HelloWorldProj_1k564
====================

This is the project.


Run Project Locally
-------------------

- First time setup:
	- Install VirtualBox (virtualbox.org) & Vagrant (vagrantup.com).
	- Run `vagrant box add laravel/homestead`
	- Add contents of "https://github.com/laravel/homestead" repo into "/vagrant_dir"
	- Create "vagrant_dir/Homestead.yaml" from "vagrant_dir/Homestead_TEMPLATE.yaml"
- Run `cd vagran_dir`, `vagrant up`
- (TBD: run a proj build script that e.g. pulls in dependencies?)
- Point web browser to local webserver at "192.168.10.10"


Publish project to Prod
-----------------------
- SSH to prod server/environment
- First time setup:
	- `git clone --depth 1 REPO_URL`
- `cd` to REPO_PROJ_DIR
- `git pull --depth 1`
- (TBD: run a proj build script that e.g. pulls in dependencies?)
- `python buildMe/deploy.py "TARGET_DIR"` (TARGET_DIR = dir that's hosted)
- (Recommend scripting above steps per your particular env.)

