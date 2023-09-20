
eg: 
terraform.tf ---> write the code to create resouce

execution command to execute the resouce:

terraform provider -> to see the provider eg: aws, github etc.
terraform init -> initilize the provider 
terraform plan -> this command say if we do execute apply command what should be change.
terraform apply -> execute the resouce or created resource which is written in tf file  
terraform apply --auto-approve -> execute the resouce or created resource which is written in tf file and no need to confirm  
terraform destroy -> delete all resouce which are created.
terraform destroy -->target github_repository.terraform-second-repo -> it will delete targeted resouce or single resouce.
terraform validate -> check the configuration are alright or not
terraform refesh -> it update what we change in created resource eg: description change Manually of github and we run refresh command it 
                    will reflect in trraform.tfstate file automatically but what we configuration done in repositoriest.tf 
                    if we apply then again delete previous repo and create new one configuration taken from repositoriest.tf file.
terraform show -> it will show terraform.tfstate in console.
terraform console -> this command used for debugging purpose what value come form variable
                    eg: after execute command then it open new console
                    eg1 -> var.username  -> it print what username come
                    eg2 -> github_repository.terraform-first-repo.html_url
                    eg3 -> github_repository.terraform-first-repo.ssh_clone_url

terraform fmt -> this command used to code formatter for all files