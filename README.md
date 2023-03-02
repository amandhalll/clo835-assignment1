### Create SSH key pair
```ssh-keygen -t rsa```

Press enter thrice after running this command

### Clone Repo
```git clone https://github.com/amandhal/ec2_ecr.git```

### Change directory to ec2_ecr
```cd ec2_ecr```

### Deploy Infrastructure
```terraform init```

```terraform apply --auto-approve```

### Login to EC2 instance
```ssh -i ~/.ssh/id_rsa ec2-user@<public_ip>```

Replace public_ip with the actual public_ip of your deployed EC2 instance

### Logout and log back in to make the docker permissions effective
