# **sample_varibles**



#### This repo is a guideline on HOW to use null provider with variables in terraform using Ubuntu.

Terraform supports several collection variable types.

    List: A sequence of values of the same type.
    Map: A lookup table, matching keys to values, all of the same type.
    Set: An unordered collection of unique values, all of the same type.
Variable blocks have three optional arguments.

    Description: A short description to document the purpose of the variable.
    Type: The type of data contained in the variable.
    Default: The default value.

# **Repo content**
```main.tf``` - Terraform configuration file

```variables.tf``` -Terraform file containing the variables 

# **PreRequsits**
#### You need to have terraform cli instaled 
#### [download link](https://www.terraform.io/downloads)

# **How to use**
```
    Download the repo igabrpro/sample_variables git clone https://github.com/igabrpro/sample_variables.git
    Change to Count_null_provider: cd Count_null_provider
    Type in your terminal terraform init in order to be downloaded required providers
    Type in your terminal terraform plan in order to see the changes which terraform is going to be made
    Type in your terminal terraform apply execute changes bases on our code(main.tf) 
```
    
    
# **Expected results**
```

null_resource.igabr[0]: Creating...
null_resource.igabr[1]: Creating...
null_resource.igabr[0]: Creation complete after 0s [id=8095310575152695955]
null_resource.igabr[1]: Creation complete after 0s [id=3764287859555020344]
```
# **Example**

```
Execute terraform show to check the created objects

# null_resource.igabr[0]:
resource "null_resource" "igabr" {
    id = "8095310575152695955"
}

# null_resource.igabr[1]:
resource "null_resource" "igabr" {
    id = "3764287859555020344"
}
```
