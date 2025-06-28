# ToolGrad: Efficient Tool-use Dataset Generation with Textual “Gradients”


This is an official, anonymous repo for the paper submission of <ToolGrad: Efficient Tool-use Dataset Generation with Textual “Gradients”>.

## ToolBench Setups

### ToolBench API Key
You need to first obtain a ToolBench API key by following their instruction:
- https://github.com/OpenBMB/ToolBench

Once you receive the API key, and do 
```bash
export TOOLBENCH_KEY=YOURTOOLBENCHKEY
```
### ToolBench API Configs
- Download [this zip file](https://drive.google.com/file/d/1mPSuXHs3weGtpla8Qs1peJccN07X-K1c/view?usp=sharing). 
- Unzip it and it will show a `tools/` folder.
- change the `LIBRARY_ROOT=` to your `tools/` folder path.

## Generate your first data sample on ToolBench using the ToolGrad framework
### Clone & Install

```bash
git clone https://github.com/user-id-123/toolgrad
cd toolgrad
conda create -n "toolgrad"
conda activate toolgrad
pip install -r requirements.txt
```
### Start generation
```bash
export PYTHONPATH=./
python examples/toolgrad_on_toolbench.py
```
You will then find a new json file under `examples/outputs/`.


