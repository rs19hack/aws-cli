**To list policies for an IAM user**

The following ``list-user-policies`` commmand lists the policies that are attached to the IAM user named ``Bob``::

  aws iam list-user-policies --user-name Bob

Output::
  	
  [
    "ExamplePolicy",
    "TestPolicy"
  ]
  
For more information, see `Adding a New User to Your AWS Account`_ in the *Using IAM* guide.

.. _Adding a New User to Your AWS Account: http://docs.aws.amazon.com/IAM/latest/UserGuide/Using_SettingUpUser.html





