# 📄 DocuMind

**DocuMind** is a minimalist documentation generator for "orphan scripts". It scans your single-file scripts (Python, JS, Bash, etc.) and generates a beautiful `README.md` based on special comment tags.

## 🚀 Features

- **Tag-based Extraction**: Uses `@description`, `@usage`, and `@arg` tags to build documentation.
- **Fast & Simple**: No complex configuration files needed.
- **Multi-language**: Works with any text-based script file.

## 🛠 Installation

```bash
pnpm install
```

## 📖 How to use

Add tags to your script:

```javascript
// @description This script backups your database to S3.
// @usage node backup.js --bucket my-bucket
// @arg --bucket: The name of the S3 bucket.
// @arg --region: AWS region (default: us-east-1).
```

Run DocuMind:

```bash
npx ts-node index.ts path/to/your/script.js > README.md
```

## 📄 License

MIT
