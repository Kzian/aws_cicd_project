# aws_cicd_project
CI/CD pipeline with GitHub Actions deploying to AWS
# AWS CI/CD Project

This repo demonstrates **CI/CD with GitHub Actions** deploying to **AWS S3**.

## Features
- Auto **version bumping & tagging** (`bump-version.yml`)
- Auto **release creation** (`create-release.yml`)
- **Deployment pipeline** to AWS S3 (`deploy-aws.yml`)

## Setup
1. Fork/clone this repo.
2. Add AWS secrets in GitHub:
   - `AWS_ACCESS_KEY_ID`
   - `AWS_SECRET_ACCESS_KEY`
   - `S3_BUCKET` (your bucket name)
   - `AWS_REGION`
3. Push code → GitHub Actions runs automatically.

## Deployment
On every push to `main`:
- App files are uploaded to your AWS S3 bucket.
- Tags & releases are auto-generated.

## License
MIT
