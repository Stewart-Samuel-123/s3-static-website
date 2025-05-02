# S3 Static Website Hosting

This project demonstrates how to host a static HTML website using Amazon S3.

---

## 🌐 What I Did

- Created a new S3 bucket with a unique name
- Enabled static website hosting in the bucket properties
- Uploaded an `index.html` file
- Configured public access settings and applied a bucket policy

---

## 📄 Example Bucket Policy

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}
