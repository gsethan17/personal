# Create virtual env on conda.
`conda create -n {env_name} python={version_of_python}`. 
`conda create -n tf python=3.8`

# activate virtual env
`conda activate [env_name}`

# install tensorflow dependencies from apple conda chennel.
`conda install -c apple tensorflow-deps`

# Install base tensorflow
`python -m pip install tensorflow-macos`

# Install apple's tensorflow-metal for GPU acceleration.
`python -m pip install tensorflow-metal`

# Check the list of available physical devices
```
import tensorflow as tf
print(tf.config.list_physical_devices()
```
