# importing-existing

## 1.2 Deliverable 

```
manning-importing-cloud-infra-into-terraform git:(main) ✗ aws iam list-users | jq '.[] | length'
103
```

After removing the state file and trying an `apply` again.

Example one of 100
```
Error: Error creating IAM User user-92-terraform: EntityAlreadyExists: User with name user-92-terraform already exists.
│       status code: 409, request id: 3965715c-379b-4dcd-900d-d43d9aeb59b5
│ 
│   on modules/cloudesk-user/user.tf line 1, in resource "aws_iam_user" "user":
│    1: resource "aws_iam_user" "user" {
```