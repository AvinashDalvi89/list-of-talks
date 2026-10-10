## Watching Self-Repair Happen: Automatic Detection and Recovery on ECS Managed Instances

### Abstract 
GPU inference breaks in ways CPUs do not. A memory error. A card that drops off the bus. A bad connection between GPUs. These faults happen at scale, not sometimes, but always.

On a self-managed fleet, nothing catches this automatically. You write a script to check GPU health. You set a CloudWatch alarm. You write a Lambda function to remove the bad instance from the load balancer. Then you refresh the instance by hand or with another script. Every step is one more place things can fail.

I wanted to see what changes with ECS Managed Instances. I injected a real GPU fault, the same kind that happens in production, into a live cluster. Then I watched what ECS did on its own. No script. No alarm I built. No manual step.

In this talk, I walk through what I saw. How ECS detects the fault using NVIDIA DCGM. How it drains the bad instance and brings up a new one before removing the old one. What this looks like in CloudWatch and EventBridge, so you know where to look when it happens to you. And where this fits, and where it does not, in a real deployment pipeline.

### Reference
- https://github.com/aws-samples/sample-ecs-inference-pipeline/tree/main/demos/gpu-auto-repair
- https://aws.amazon.com/blogs/containers/graceful-shutdowns-with-ecs/
