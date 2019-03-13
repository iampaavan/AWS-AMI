# AWS AMI for CSYE 6225

## Team Information

| Name | NEU ID | Email Address |
| Hemalkumar Gadhiya | 001460477 | gadhiya.h@husky.neu.edu |
| Paavan Gopala reddy | 001813403 | gopalareddy.p@husky.neu.edu |
| Satish Kumar Anbalagan | 001351994 | anbalagan.s@husky.neu.edu |
| Akshay Murgod | 001635872 | murgod.a@husky.neu.edu |

## Validate Template

```
packer validate ubuntu-ami.json
```
packer validate centos-ami-template.json

## Build AMI

```
packer build \
    -var 'aws_access_key=REDACTED' \
    -var 'aws_secret_key=REDACTED' \
    -var 'aws_region=us-east-1' \
    -var 'subnet_id=REDACTED' \
    centos-ami-template.json
```

#
