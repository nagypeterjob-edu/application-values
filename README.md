# application-values
#TheSpinnakerCourse - storing helm values and global namespace overrides

# AWS permissions

Permissions needed for the (travis) deploy script to work:
```json
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Resource": [
                "arn:aws:s3:::yourbucket",
                "arn:aws:s3:::yourbucket/*"
            ],
            "Effect": "Allow",
            "Action": [
                "s3:DeleteObject",
                "s3:GetBucketLocation",
                "s3:GetObject",
                "s3:ListBucket",
                "s3:PutObject",
                "s3:PutObjectAcl"
            ]
        }
    ]
}
```
