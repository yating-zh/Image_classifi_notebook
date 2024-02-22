## Conda command should know

1. Set the conda's base environment not be activated on startup:
> $ conda config --set auto_activate_base false

2. To activate Conda environment:
> $ conda activate base
> $ conda activate tensorflow (tensorflow is the name of the env)

3. List all the conda environment
> $ conda env list

4. Activate a environment(base)
> $ conda activate base

5. Remove a conda environment - switch to another env(eg:base) then remove the specific env (eg: name is envv)
> $ conda activate base

> $ conda env remove --name envv

6. Switch back to system (local) environment
>$ conda deactivate
