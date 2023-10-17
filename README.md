# 2023-02-02, -03

# Repository sv-security-scans-01

Internal(?) repository for security scans, by Sergei Vorobyov.

Contains different workflows in `.github/workflows` for a number of 
security scans, which you can borrow into your own workflows.

## What Is Included

1. Subdirectory `terraform-in-action/` contains sample code from the 
book 'Terraform in Action', copied from the author's GitHub repository
https://github.com/terraform-in-action/manning-code. Used for sample scans.
2. Subdirectory `./github/workflows/` contains sample workflows, for 
different security scans.
3. You may inspect workflow runs, for `Checkov` (Palo Alto) and 
`TFSec` (AquaSec) on the sample Terraform code in
https://github.com/.../sv-security-scans-01/actions
4. All our workflows are in the default directory
`.github/workflows/`


### `checkov-01.yml`

Sample workflow running Palo Alto Checkov IaC scanner, on a chapter 
of the book 'Terraform in Action'.

### `tfsec-01.yml`

Sample workflow running AquaSec TFSec IaC scanner, on a chapter
of the book 'Terraform in Action'.

### `trivy-01-image.yml`

Sample workflow running AquaSec Trivy scan in **image** mode.
Uses the mainstream DockerHub image `ubuntu:latest` as scan target.
Finds a few Medium and Low vulnerabilities from CVE (Common Vulnerabilities 
and exposures).

### `trivy-02-fs.yml`

Sample workflow running AquaSec Trivy scan in **fs** (file 
system) mode.

### `pip-audit-01.yml`

Sample workflow with Python dependencies vulnerabilities scan.


### `gitleaks-01.yml`

...

### `lgtm-01.yml`

Discontinued/retired/deprecated:
https://github.blog/2022-08-15-the-next-step-for-lgtm-com-github-code-scanning/
Ignore
(16th of December 2022: LGTM.com will be shut down)


### `.yml`
