## Physics Simulation Engine for Real Env
Zhiyang He

### Requirements
Physics simulation is tested to work on both python 2 and 3.

Install dependencies inside environment
```shell
source activate (env_name)
pip install pybullet, zmq, transforms3d
```

Make proper obj file for OpenGL convention
```
python invert_obj --datapath ../data --model model_id
```


### Run the code
Simply running this will not do anything, because now physics renderer is tied together with view renderer. You should not be running standalone view renderer either
```shell
python render_physics.py --datapath ../data --model model_id
```
