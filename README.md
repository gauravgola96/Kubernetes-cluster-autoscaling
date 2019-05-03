# Kubernetes-cluster-autoscaling
Use this yaml file to create a cluster autoscaling deployment on AWS.

NOTE : You have to add your node to AWS AUTOSCALING GROUP.

Changes to made in yaml file :-
1) Add MAX_NODE and MIN_NODE : This should match with your Aws autoscaling group  https://docs.aws.amazon.com/autoscaling/ec2/userguide/AutoScalingGroup.html

2) AWS AUTOSCALING GROUP : Name of your ASG group (On which you have added your node)

3) AWS_REGION

COMMAND: 
kubectl create -f cluster-autoscaler.yaml --namespace XXX
