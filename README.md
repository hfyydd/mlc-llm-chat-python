# mlc-llm-chat-python 
### I tweaked some parts of the chat.py file to running. The file is from [mlc-llm](https://github.com/mlc-ai/mlc-llm/blob/main/tests/chat.py) 
## Test on MacBook Air M2 16GB

Follow these steps to run mlc-llm chat.py

## Step 1: Compile TVM
tvm relax
```bash
git clone https://github.com/mlc-ai/relax.git --recursive
```
Then try 
```python
import tvm
from tvm import relax
```


## Step 2: Download LLM Weights and libs 
```bash
mkdir -p dist
git lfs install
git clone https://huggingface.co/mlc-ai/demo-vicuna-v1-7b-int3 dist/vicuna-v1-7b
git clone https://github.com/mlc-ai/binary-mlc-llm-libs.git dist/lib
```
## Step 3: Copy the dist folder and [mlc_llm](https://github.com/mlc-ai/mlc-llm/tree/main/mlc_llm) folder into the project directory.

## Step 4: Run the chat.py

To run the project, execute the following command:

```bash
python chat.py
```
Then You can chat with LLM or do something with python !
