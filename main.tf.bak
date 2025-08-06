resource "null_resource" "ambiente" {
  provisioner "local-exec" {
    command = "echo Estoy en el workspace ${terraform.workspace}"
  }
}

terraform {
  backend "remote" {
    organization = "terraform-demo-practice"

    workspaces {
      name = "terraform-course-cloud"
    }
  }
}