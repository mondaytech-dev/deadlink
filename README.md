<p align="center">
  <a href="https://github.com/mondaytech-dev/deadlink"><img alt="deadlink" src="https://raw.githubusercontent.com/mondaytech-dev/deadlink/refs/heads/main/images/deadlink-logo-with-text.svg" width="60%"></a>
</p>

[![PyPi Version](https://img.shields.io/pypi/v/deadlink.svg?style=flat-square)](https://pypi.org/project/deadlink/)
[![PyPI pyversions](https://img.shields.io/pypi/pyversions/deadlink.svg?style=flat-square)](https://pypi.org/project/deadlink/)
[![GitHub stars](https://img.shields.io/github/stars/mondaytech-dev/deadlink.svg?style=flat-square&logo=github&label=Stars&logoColor=white)](https://github.com/mondaytech-dev/deadlink/)
[![Downloads](https://static.pepy.tech/badge/deadlink/month?style=flat-square)](https://pepy.tech/projects/deadlink)

Parses text files for HTTP URLs and checks if they are still valid. Install with

```
pip install deadlink
```

and use as

```sh
deadlink check README.md   # or multiple files/directories
# or deadlink c README.md
```

You can configure deadlink via its config file
`~/.config/deadlink/deadlink.toml`, e.g.,

```toml
timeout_s = 10
cache_ttl_s = 259200
num_concurrent_requests = 5
# allow_file_extensions = ["txt", "yaml", "c"]
ignore_hosts = ["www.example.com"]
```

Example output:

<!--screenshot created with https://carbon.now.sh/-->

![](https://raw.githubusercontent.com/mondaytech-dev/deadlink/refs/heads/main/images/example-output-carbon.png)
