# Requirements
- terraform

# How to start
- Create a folder and then enter, create a new file called "main.tf" and write this code <br>
    resource "kind-of-file" "name" { <br> <br> } <br>
- Change the "kind-of-file" for "local_file" because we are work in our local and change the name for example or test, you choose <br>
- Inside the resource that you are creating, specify what will do, we can include a filename called "example.txt" and also include the unique and one "Hello World" inside the file <br>
- We will have something like this <br>
    resource "local_file" "example" { <br> filename = "example.txt" <br> content = "Hello World" <br> } <br>
- After save your file, we can start, run this commands in order and see the terminal <br>
- terraform version <br>
- terraform init <br>
- terraform plan <br>
- terraform apply <br>

- The init command will create a terraform file with a kind of checkpoint called .terraform.lock.hcl <br>
- The plan will show you what are you executing and if you have more steps, will advise you notifying how many changes you will apply <br>
- The apply will execute your resource and will create/destroy what you are specyfing in your files<br>

- Congrats, we create a file called "example.txt" and says "Hello World"