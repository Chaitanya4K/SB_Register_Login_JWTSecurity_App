# AWS S3 Static Website Hosting

## Project Overview

This project demonstrates how to build a static website using HTML and CSS and host it on Amazon Web Services (AWS) S3. It also provides an opportunity to practise Git, GitHub, and Jenkins for source control and continuous integration (CI).

## Technologies Used

- **HTML5** — Website structure
- **CSS3** — Website styling
- **Amazon S3** — Static website hosting
- **Git & GitHub** — Source code management and version control
- **Jenkins** — CI pipeline and automated file validation

## Project Objectives

- Build a static website using HTML and CSS.
- Host website files using an Amazon S3 bucket.
- Understand S3 static website hosting.
- Manage project source code using Git and GitHub.
- Configure Jenkins to fetch source code from GitHub.
- Validate website files through a Jenkins pipeline.

## Project Structure

```text
Mini-Project-AWS-S3-Static-Website/
├── index.html
├── courses.html
├── contact.html
├── error.html
├── style.css
├── README.md
├── .gitignore
└── Jenkinsfile
```

*Adjust the file list to match the files actually present in your repository.*

## AWS S3 Deployment

1. Sign in to the AWS Management Console.
2. Open Amazon S3.
3. Create a uniquely named S3 bucket in your preferred AWS Region.
4. Upload the website's HTML, CSS, and other required assets.
5. Configure static website hosting and select `index.html` as the index document.
6. Configure access according to your learning requirements and AWS security best practices.
7. Open the S3 website endpoint to test the website.

**Security note:** Public website access may require a bucket policy and public-access settings. Review the security implications before enabling public access. S3 website endpoints do not provide HTTPS by themselves.

## Jenkins CI Integration

The Jenkins pipeline can automate basic validation of the website source code.

### Pipeline stages

1. **Checkout:** Retrieve the source code from GitHub.
2. **File Validation:** Verify that required website files exist.
3. **HTML Validation:** Perform basic checks on HTML files.
4. **Build Result:** Report success or failure in Jenkins.

### Jenkins setup

1. Push the project to GitHub, including the `Jenkinsfile`.
2. Create a Pipeline job in Jenkins.
3. Configure the GitHub repository URL under Pipeline from SCM.
4. Select the `main` branch.
5. Set the script path to `Jenkinsfile`.
6. Run the job and review the Console Output.

> The initial pipeline validates source files. It does not deploy the website to S3 unless an S3 deployment stage is added.

## How to Run Locally

1. Clone the repository:

   ```bash
   git clone YOUR_GITHUB_REPOSITORY_URL
   ```

2. Open the project folder.

3. Open `index.html` in a web browser.

4. Navigate through the website pages and verify that the styling works correctly.

## Learning Outcomes

- Static website hosting with Amazon S3
- Basic AWS storage and access configuration
- Git and GitHub repository management
- Jenkins Pipeline fundamentals
- Automated source-code validation
- Introduction to CI/CD workflows

## Future Improvements

- Add automated HTML validation using a dedicated validator.
- Configure Jenkins to deploy website files to S3.
- Add deployment approval and error handling.
- Configure HTTPS and a custom domain using appropriate AWS services.
- Improve responsive design and accessibility.

## Author

**Chaitanya4K**

Java Developer | Spring Boot | AWS | Docker | Jenkins | Kubernetes

## License

This project is intended for learning and portfolio demonstration. Add a license file if you want to specify permissions for reuse and distribution.
