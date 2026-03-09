# GitHub Actions Workflows Collection 🚀

![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF)
![CI/CD](https://img.shields.io/badge/CI%2FCD-Professional-blue)

A collection of production-ready GitHub Actions workflows for modern web applications.

## 📦 Included Workflows

### 1. CI (ci.yml)
- Multi-version Node.js testing (18.x, 20.x, 22.x)
- Linting and type checking
- Unit tests with coverage
- Codecov integration

### 2. Deploy (deploy.yml)
- Production deployment
- Vercel integration
- Environment secrets management

### 3. Release (release.yml)
- Semantic versioning
- Release drafter
- Auto npm publishing

## 🚀 Quick Start

```bash
# Clone the repository
gh repo clone 553226713/github-actions-workflows

# Copy the workflow you need to your repository
cp .github/workflows/ci.yml your-repo/.github/workflows/
```

## 📚 Workflows Overview

| Workflow | Trigger | Purpose |
|----------|---------|---------|
| CI | Push/PR | Run tests, linting, type check |
| Deploy | Push to main | Deploy to production |
| Release | Tag push | Create release & publish npm |

## 🔧 Required Secrets

For deployments, add these secrets to your GitHub repository:

```
VERCEL_TOKEN
VERCEL_ORG_ID
VERCEL_PROJECT_ID
CODECOV_TOKEN
NPM_TOKEN
```

## 📝 Usage Examples

### Use with npm workspaces
```yaml
- name: Install dependencies
  run: npm ci --workspaces
```

### Use with pnpm
```yaml
- name: Setup pnpm
  uses: pnpm/action-setup@v2
  with:
    version: 8

- name: Install dependencies
  run: pnpm install --frozen-lockfile
```

## 🎯 Pro Version

Get the **Pro Version** with additional workflows:

- 🐳 Docker build & push
- ☁️ AWS deployment
- 🔒 Security scanning
- 📊 Performance testing
- 📱 Mobile app builds

[Buy Pro Version →](https://gum.co/gh-actions-pro)

## ❤️ Support

If this template helps you, please consider:

- ⭐ **Star** this repository
- 🐛 **Report** issues
- 🔧 **Submit** pull requests

[![GitHub Sponsors](https://img.shields.io/badge/Sponsor-❤-ea4aaa?style=flat&logo=github-sponsors)](https://github.com/sponsors/553226713)

## 💰 支持一下

如果这个项目对你有帮助，可以扫码打赏支持！

<img src="https://raw.githubusercontent.com/553226713/github-actions-workflows/main/alipay.png" width="200" alt="支付宝收款码"/>

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

MIT License

---

<div align="center">
  <p>Made with ❤️ by <a href="https://github.com/553226713">553226713</a></p>
</div>
