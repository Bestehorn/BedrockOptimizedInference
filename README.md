# Bedrock Optimized Inference Notebook
This repository contains a notebook that I created for measuring the performance of Bedrock standard inference (on-demand) vs the optimized performance feature that was released at re:invent 2024: https://aws.amazon.com/about-aws/whats-new/2024/12/latency-optimized-inference-foundation-models-amazon-bedrock/
The feature allows customers to decrease their latency-sensitive Generative AI solutions to use a "priority treatment", so that responses are delivered even faster than with standard latency.

**Important**: The notebook requires an AWS security context to properly access the Bedrock converse() API. I recommend running this inside a Sagemaker Studio notebook (or similar) with an IAM role attached that has adequate permissions to access Bedrock.  
