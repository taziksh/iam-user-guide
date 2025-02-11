# IAM: Access the policy simulator console<a name="reference_policies_examples_iam_policy-sim-console"></a>

This example shows how you might create an IAM policy that allows using the policy simulator console for policies attached to a user, group, or role in the current AWS account\. This policy grants the permissions necessary to complete this action programmatically from the AWS API or AWS CLI\.

You can access the IAM Policy Simulator console at: [https://policysim\.aws\.amazon\.com/](https://policysim.aws.amazon.com/)

```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Action": [
                "iam:GetGroup",
                "iam:GetGroupPolicy",
                "iam:GetPolicy",
                "iam:GetPolicyVersion",
                "iam:GetRole",
                "iam:GetRolePolicy",
                "iam:GetUser",
                "iam:GetUserPolicy",
                "iam:ListAttachedGroupPolicies",
                "iam:ListAttachedRolePolicies",
                "iam:ListAttachedUserPolicies",
                "iam:ListGroups",
                "iam:ListGroupPolicies",
                "iam:ListGroupsForUser",
                "iam:ListRolePolicies",
                "iam:ListRoles",
                "iam:ListUserPolicies",
                "iam:ListUsers"
            ],
            "Effect": "Allow",
            "Resource": "*"
        }
    ]
}
```