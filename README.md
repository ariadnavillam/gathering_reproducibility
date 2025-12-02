A repository for our gathering on reproducibility on the 2nd of December 2025

# Instructions
1. Install the [uv python package manager](https://docs.astral.sh/uv/)
2. Clone the repository
3. Create a new branch locally
5. Install the environment specified by `environment.yml` using `uv`
6. Use uv to run `try_to_run_me_after_env_install.py`
7. Try adding a new dependency to the project and also to the script
8. Commit changes made to `pyproject.toml` and `uv.lock` file to your branch
9. (Optional) Push your branch to this repository (only possible for menchelab members otherwise you can also try to fork and push to your own)

# Bonus level
Once you managed to install the environment with `uv` you can try to create a container image containing the envrionment. To do so try the following
1. Make sure you have [Docker](https://www.docker.com/) (or similar like [Apptainer](https://apptainer.org/)) installed
2. Find suitable images of `uv` and a linux distribution of your choice on a registry like [docker hub](https://hub.docker.com/)
3. Use these images to generate a build script for a container (try following [this](https://devopscube.com/reduce-docker-image-size/) or [that](https://medium.com/@ksaquib/how-i-cut-docker-image-size-by-90-best-practices-for-lean-containers-1f705cead02b) guide to reduce the size of the resulting image)
4. Run the container and try to execute `try_to_run_me_after_env_install.py` again

# Happy reproducing :)
