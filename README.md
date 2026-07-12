# Unraid Third-Party Application Templates

This repository hosts community-maintained Docker XML templates for third-party servers and applications optimized for Unraid.

---

## 🚀 How to Add This Repository to Unraid

To use these templates on your Unraid server:

1. Copy the repository URL:
   ```text
   https://github.com/UberMetroid/unraid-thirdparty
   ```
2. Navigate to your Unraid WebGUI.
3. Go to the **Apps** tab (Community Applications).
4. Click on **Repositories** in the left sidebar or at the top.
5. Paste the URL into the repository input field and add it.

Once added, the applications below will appear in your Community Applications search results.

---

## 📦 Available Templates

| Application | Description & Upstream | Default Configuration |
| :--- | :--- | :--- |
| **[OpenRepo](templates/openrepo.xml)** | Package repository hosting server for Debian, RPM, and generic files. ([GitHub](https://github.com/openkilt/openrepo)) | Web UI: `8080:8080`<br>Storage: `/mnt/user/appdata/openrepo` |
| **[Gitea](templates/gitea.xml)** | A painless self-hosted Git service written in Go. ([GitHub](https://github.com/go-gitea/gitea)) | Web UI: `3000:3000`<br>SSH: `2222:22`<br>Storage: `/mnt/user/appdata/gitea` |
| **[Ollama](templates/ollama.xml)** | Run open-source large language models locally. ([GitHub](https://github.com/ollama/ollama)) | API Port: `11434:11434`<br>Storage: `/mnt/user/appdata/ollama` |
| **[Soft Serve](templates/soft-serve.xml)** | Self-hosted, user-configurable Git server for the command line. ([GitHub](https://github.com/charmbracelet/soft-serve)) | SSH Port: `23231:23231`<br>Storage: `/mnt/user/appdata/soft-serve` |


---

## 🤝 Support & Contributions

If you encounter issues or want to submit updates to these templates, please open an issue or pull request.

- **Issues**: [GitHub Issues](https://github.com/UberMetroid/unraid-thirdparty/issues)
- **Pull Requests**: [GitHub Pull Requests](https://github.com/UberMetroid/unraid-thirdparty/pulls)

---

## 📄 License

This repository is licensed under the [MIT License](LICENSE).
