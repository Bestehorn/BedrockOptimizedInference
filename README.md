# Bedrock Optimized Inference Notebook (by Markus Bestehorn)
This repository contains a notebook that I created for measuring the performance of Bedrock standard inference (on-demand) vs the optimized performance feature that was released at re:invent 2024: https://aws.amazon.com/about-aws/whats-new/2024/12/latency-optimized-inference-foundation-models-amazon-bedrock/
The feature allows customers to decrease their latency-sensitive Generative AI solutions to use a "priority treatment", so that responses are delivered even faster than with standard latency.

**Important**:
1. The notebook requires an AWS security context to properly access the Bedrock converse() API. I recommend running this inside a Sagemaker Studio notebook (or similar) with an IAM role attached that has adequate permissions to access Bedrock.
2. The code inside the notebook was written with the aim to be readable. While some of the code could use more performance-optimized constructs to reduce local resource usage, this is not the intention of the notebook.

 
**Disclaimer**: This notebook was solely created for measuring the performance of Bedrock standard inference vs. the optimized performance feature. The code is not intended for other purposes and most importantly not for production purposes.
