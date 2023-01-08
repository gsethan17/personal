# Create virtual env on conda.
`conda create -n {env_name} python={version_of_python}`. 
`conda create -n jupyter_vim python=3.8`

# activate virtual env
`conda activate {env_name}`

# install tool for extensions on jupyter notebook.
`conda install -c conda-forge jupyter_contrib_nbextensions`  
[github for jupyter extension](https://github.com/ipython-contrib/jupyter_contrib_nbextensions)

# install jupyter extension tool on local PC
`jupyter contrib nbextension install --user`

# check address of installed jupyter extension tool.
`jupyter --data-dir`  
it will return the address

# move the address
`cd {the address}/nbextensions`  
  - If there is no nbextensions folder, make the nbextensions folder as below.  
  - `cd {the address}`  
  - `mkdir nbextensions`  
  - `cd nbextensions`  

# install vim binding
`git clone https://github.com/lambdalisue/jupyter-vim-binding`  
[github for vim binding extension](https://github.com/lambdalisue/jupyter-vim-binding)

# modify vimbinding to enable
`jupyter nbextension enable jupyter-vim-binding/vim_binding`
