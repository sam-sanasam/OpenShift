### User
There are 3 types of user are avialble in the openShift 
1. Regular user
2. System user
3. Service account

#### Regular user
These are the user like developer or other user who interect more often with the Openshift for deployment

#### System user

These are the user who interect more with the infastructure such as cluster admin or user created for each nodes in the cluster

#### Service account
Created for each if requred for enabling amoung the services


The below points is important to know:\
OAuth service:
It is use to authentical all the user.
For All-in-one , the Oauth lis "allow all"
for high level cluster, its all "Deny all"

So, in order the enable the authentication or giving persion to some specific user, we can do it manually by modifying the file

```
   /ect/openshift/master/master-config.yaml
   
   ```
 #### Some command used for User
 
 ```
 $ oc get projects   # to list all the avialble porjects
 $ co get users      # to list all the user
 
```

#### TO enable or set the other user as system admin , follow the below steps
1. log in the web console giving the user and password.
2. list the user by running  
```
$ oc get users

```
3. Run 
```
$ oc adm policy add-cluster-role-user cluster-admin <user_name>
```
to do so, it is assigned the <user_name> as cluster admin 
