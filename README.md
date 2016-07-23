# Stuart Wakefield 2016 Infrastructure

Usage: first ensure that an IAM user has been set up with
the relevant permissions and that the AWS credentials for
authentication are set up in `$HOME/.aws/credentials`.

Then set up a virtual environment, install the Python
dependencies and run the build.py script:

```sh
virtualenv .venv
source .venv/bin/activate
pip install -r requirements.txt
python build.py
```

The script will expect the following environment variables:

```
ECS_AMI="your-ami"
ECS_INSTANCE_ROLE="your-instance-role-arn"
```
