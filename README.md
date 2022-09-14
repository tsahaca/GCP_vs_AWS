# GCP_vs_AWS

## Key differences

- When it comes to accessing your VM, there are a number of key differences in the approach taken between Compute Engine and Amazon EC2.
If you want terminal access to an instance in Amazon EC2 you’ll need to include your own SSH key.
Compute Engine offers a more flexible approach to terminal access. Allowing you to create an SSH key as and when you need it, even if that instance already running. You also won’t need to store these keys on your local machine, thanks to Compute Engine’s browser-based SSH terminal which is available via the Google Cloud Console.
- When it comes to image storage, they take slightly different approaches. On Google Cloud, images are stored with Compute Engine, while Amazon EC2 stores its images in different services – Amazon Simple Storage Service (S3) or Amazon Elastic Block Store (EBS).
- On the flip-side, Compute Engine offers the benefit of globally available machine images. While Amazon Machine images are geo-locked, meaning they are only available in a specific region.
- Amazon EC2 auto-scales instances in a group, with each instance created from a defined launch configuration. Instances are created or removed based on one of three chosen scaling plans

Manual – you manually instruct auto-scaling up or down
Schedule – you configure specific timeframes to auto-scale resources
Dynamic – you create policies to scale your instances based on Amazon CloudWatch metrics or Amazon Simple Queue Service (SQS) queues.
Compute Engine scales instances in a managed instance group. Each instance group is created from an instance template with resources scaled based on an autoscaling policy. Unlike Amazon EC2, Compute Engine’s auto scaler only supports dynamic scaling.



