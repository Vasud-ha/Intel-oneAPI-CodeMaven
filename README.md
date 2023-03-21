# Intel-oneAPI-CodeMaven
## Environment set up for various run:
Step 1: Open the condaenvsetup.ipynb and activate Python 3(Intel oneAPI 2022.3) kernel<br />
Step 2: Run through the cells one by one. "qsub" submits the job to do all the setup and "qstat" shows the job status. (all details related to devcloud job submission is in the Welcome.ipyb file)<br />
Step 3: Once the job is finished, the setup should be completed.<br />
Step 4: Now you will have stock-tensorflow as well as intel-tensorflow in the jupyter kernels to run the benchmark code.<br />

## Running the notebooks:
### Exercise 1: Intel® Tensorflow and Stock Tensorflow Performance Comparison 

Step 1: Open terminal, and clone oneAPI samples<br />
git clone https://github.com/oneapi-src/oneAPI-samples.git<br />
Step 2: Browse the oneAPI-samples/AI-and-Analytics/Features-and-Functionality/IntelTensorFlow_ModelZoo_Inference_with_FP32_Int8/<br />
Step 3: Open the ResNet50_Inference.ipynb<br />
Step 4: First select stock-tensorflow kernel and add the following env variable [os.environ["TF_ENABLE_ONEDNN_OPTS"]='0'] to disable onednn and run through each cell of the notebook to get the average time and throughput.<br />
Step 5: Follow step 4 but now with onednn on by changing the env variable  [os.environ["TF_ENABLE_ONEDNN_OPTS"]='1'] and note the performance<br />
Step 6: Repeat the same process but this time with intel-tensorflow kernel to add further openmp optimizations and compare the average time and throughput<br />


## Documentation Links:

Intel® Devcloud for oneAPI documentation
https://devcloud.intel.com/oneapi/get_started/
