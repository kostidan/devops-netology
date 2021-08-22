# devops-netology
#### Local .terraform directories
\**/.terraform/\* - исключить все файлы, находящиеся в любой поддиректории с именем .terraform

#### .tfstate files
\*.tfstate - исключить все файлы в текущей директории, имя которых заканчивается на .tfstate

\*.tfstate.\* - исключить все файлы в текущей директории, имя которых содержит .tfstate.

#### Crash log files
crash.log - исключить файл crash.log в текущей директории

#### Exclude all .tfvars files, which are likely to contain sentitive data, such as
#### password, private keys, and other secrets. These should not be part of version
#### to change depending on the environment.
####
\*.tfvars - исключить все файлы в текущей директории, имя которых заканчивается на .tfvars

#### Ignore override files as they are usually used to override resources locally and so
#### are not checked in
override.tf - исключить файл override.tf в текущей директории

override.tf.json - исключить файл override.tf.json в текущей директории

\*_override.tf - исключить все файлы, имя которых оканчивается на _override.tf в текущей директории

\*_override.tf.json - исключить все файлы, имя которых оканчивается на _override.tf.json в текущей директории


#### Include override files you do wish to add to version control using negated pattern
#### !example_override.tf

#### Include tfplan files to ignore the plan output of command: terraform plan -out=tfplan
#### example: *tfplan*

#### Ignore CLI configuration files
.terraformrc - исключить файл .terraformrc в текущей директории

terraform.rc - исключить файл terraform.rc в текущей директории

