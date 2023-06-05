# Functionality

|**API**| **Category** | **Supported data type** | 
|-------|--------------|-------------------------|
| xetla::gemm | GEMM | bf16, fp16, fp32, tf32 |
| xetla::brgemm | GEMM | bf16, fp16, fp32, tf32 |
| xetla::epilogue | GEMM | bf16, fp16, fp32, tf32 |
| xetla::layer_norm |REDUCE  | bf16, fp16, fp32, tf32 |
| xetla::row_reduction |REDUCE | fp32 |
| xetla::group_reduction |REDUCE  | fp32 |
| xetla::data_convert |DATA  | bf16, fp16, fp32, tf32 |
| xetla::tile | UTIL | bf16, fp16, fp32, tf32 |
| xetla::core | UTIL | bf16, fp16, fp32, tf32 |
 
 
#### GEMM 

|**API**| **Category** | **Input data type **| **TRANSPOSE** | **Compute Unit** |  
|-------|--------------|--------------------|--------------|--------------|
| xetla::GEMM | GEMM |  | bf16:bf16:fp32  | NN, NT, TN | DPAS, FMA |

#### Epilogue 

|**API**| **Category** | **Input data type **| **TRANSPOSE** | **Compute Unit** |  
|-------|--------------|--------------------|--------------|--------------|
 
 #### Reduction

|**API**| **Category** | **Input data type **| **TRANSPOSE** | **Compute Unit** |  
|-------|--------------|--------------------|--------------|--------------|
 
 #### Data Convert 

|**API**| **Category** | **Input data type **| **TRANSPOSE** | **Compute Unit** |  
|-------|--------------|--------------------|--------------|--------------|
 
 
 
 ## Terms

- N - Column Major
- T - Row Major
- {N|T, N|T} - describe whether the matrix is transposed or not
- FP32 - single float representation
- BF16 - half precision of bfloat16 
- FP16 - half precision of float
- TF32 - tensor float 
- FP8 - 8 bits float precision 
- FMA - float multiple addition
- DPAS - 
