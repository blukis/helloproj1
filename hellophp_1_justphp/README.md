HelloWorldProj_1k564
====================

This is the project.

Run Project Locally
-------------------

- First time setup:
	- Add contents of "https://github.com/laravel/homestead" repo into "/vagrant_dir"
	- Create "vagrant_dir/Homestead.yaml" from "vagrant_dir/Homestead_TEMPLATE.yaml"
	- Install vagrant, virtualbox
	- Run `vagrant box add laravel/homestead`
- From /vagran_dir, run `vagrant up`
- Point web browser to local webserver at "192.168.10.10"

Publish project to Prod
-----------------------
- SSH to prod server/environment
- First time setup only:
	- `git clone --depth 1 REPO_URL`
- `cd` to REPO_PROJ_DIR
- `git pull --depth 1`
- `python buildMe/deploy.py "TARGET_DIR"` (TARGET_DIR = dir that's hosted)
- Recommend scripting above steps per your particular env.

